# Comparing `tmp/flwr_nightly-1.5.0.dev20230719.tar.gz` & `tmp/flwr_nightly-1.5.0.dev20230720.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.5.0.dev20230719.tar", max compression
+gzip compressed data, was "flwr_nightly-1.5.0.dev20230720.tar", max compression
```

## Comparing `flwr_nightly-1.5.0.dev20230719.tar` & `flwr_nightly-1.5.0.dev20230720.tar`

### file list

```diff
@@ -1,112 +1,112 @@
--rw-r--r--   0        0        0    11358 2023-07-19 23:00:57.175891 flwr_nightly-1.5.0.dev20230719/LICENSE
--rw-r--r--   0        0        0    10808 2023-07-19 23:00:57.175891 flwr_nightly-1.5.0.dev20230719/README.md
--rw-r--r--   0        0        0     5434 2023-07-19 23:01:18.112207 flwr_nightly-1.5.0.dev20230719/pyproject.toml
--rw-r--r--   0        0        0      952 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/__init__.py
--rw-r--r--   0        0        0     1164 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    14058 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     7677 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     7209 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      728 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     4954 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      745 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     7345 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0      712 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     6380 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     4693 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     5318 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      728 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0     9050 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0     2877 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1875 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     1113 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0      884 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     1791 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     1889 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     3459 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0     2120 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0    16315 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7805 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     3714 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      848 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      809 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/driver/__init__.py
--rw-r--r--   0        0        0     4826 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/driver/app.py
--rw-r--r--   0        0        0     3906 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/driver/driver.py
--rw-r--r--   0        0        0     4877 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/driver/driver_client_manager.py
--rw-r--r--   0        0        0     5653 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/driver/driver_client_proxy.py
--rw-r--r--   0        0        0      676 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     4663 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     3815 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     5727 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     1617 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     7295 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     6182 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0     7505 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     2183 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1188 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     8232 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0    10889 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 23:00:57.555895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0    18721 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1370 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    26333 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6120 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2227 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0     1054 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      705 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     3919 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/driver/driver_servicer.py
--rw-r--r--   0        0        0      704 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/__init__.py
--rw-r--r--   0        0        0      728 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     4467 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
--rw-r--r--   0        0        0     5686 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6408 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4650 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11501 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0     6313 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
--rw-r--r--   0        0        0      751 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     2546 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0      724 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     2876 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      728 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     3686 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0     4897 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/history.py
--rw-r--r--   0        0        0    15958 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/server.py
--rw-r--r--   0        0        0      996 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/state/__init__.py
--rw-r--r--   0        0        0     6774 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/state/in_memory_state.py
--rw-r--r--   0        0        0    19294 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/state/sqlite_state.py
--rw-r--r--   0        0        0     4833 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/state/state.py
--rw-r--r--   0        0        0     1647 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/state/state_factory.py
--rw-r--r--   0        0        0     1667 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0     6099 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     4654 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     6995 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5893 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6740 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7014 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11522 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9991 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8286 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2708 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5428 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     7126 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     6026 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     3519 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     7079 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6343 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10154 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7484 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      901 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5478 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     4940 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0     1271 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0     7762 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      727 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0     5471 2023-07-19 23:00:57.559895 flwr_nightly-1.5.0.dev20230719/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0    13130 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230719/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-20 23:00:43.622921 flwr_nightly-1.5.0.dev20230720/LICENSE
+-rw-r--r--   0        0        0    10808 2023-07-20 23:00:43.622921 flwr_nightly-1.5.0.dev20230720/README.md
+-rw-r--r--   0        0        0     5484 2023-07-20 23:01:00.431167 flwr_nightly-1.5.0.dev20230720/pyproject.toml
+-rw-r--r--   0        0        0      952 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0     1164 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    14058 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     7677 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     7209 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      728 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     4954 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      745 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     7345 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0      712 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     6380 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     4693 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     5318 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      728 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0     9050 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0     2877 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1875 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     1113 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0      884 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     1791 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     1889 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     3459 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0     2120 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0    18778 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7805 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     3861 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      848 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      809 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/driver/__init__.py
+-rw-r--r--   0        0        0     4826 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/driver/app.py
+-rw-r--r--   0        0        0     3906 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/driver/driver.py
+-rw-r--r--   0        0        0     4877 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/driver/driver_client_manager.py
+-rw-r--r--   0        0        0     5653 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/driver/driver_client_proxy.py
+-rw-r--r--   0        0        0      676 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     4663 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     3815 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     5727 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     1617 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7295 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     6182 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0     7505 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     2183 2023-07-20 23:00:44.086927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1188 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8232 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0    10889 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18721 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1370 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    26333 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6120 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2227 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0     1054 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      705 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     3919 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/driver/driver_servicer.py
+-rw-r--r--   0        0        0      704 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/__init__.py
+-rw-r--r--   0        0        0      728 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     4467 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
+-rw-r--r--   0        0        0     5686 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6408 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4650 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11501 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0     6313 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
+-rw-r--r--   0        0        0      751 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     2546 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0      724 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     2876 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      728 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     3686 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0     4897 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0    15958 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0      996 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/state/__init__.py
+-rw-r--r--   0        0        0     6774 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/state/in_memory_state.py
+-rw-r--r--   0        0        0    19294 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/state/sqlite_state.py
+-rw-r--r--   0        0        0     4833 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/state/state.py
+-rw-r--r--   0        0        0     1647 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/state/state_factory.py
+-rw-r--r--   0        0        0     1667 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0     6099 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     4654 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     6995 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5893 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6740 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     7014 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11522 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9991 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8286 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2708 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5428 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     7126 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     6026 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     3519 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     7079 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6343 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10154 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7484 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      901 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5478 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     5672 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0     1271 2023-07-20 23:00:44.090927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0     7762 2023-07-20 23:00:44.094927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      727 2023-07-20 23:00:44.094927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0     5471 2023-07-20 23:00:44.094927 flwr_nightly-1.5.0.dev20230720/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0    13223 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230720/PKG-INFO
```

### Comparing `flwr_nightly-1.5.0.dev20230719/LICENSE` & `flwr_nightly-1.5.0.dev20230720/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/README.md` & `flwr_nightly-1.5.0.dev20230720/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
    [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb))
 
 Stay tuned, more tutorials are coming soon. Topics include **Privacy and Security in Federated Learning**, and **Scaling Federated Learning**.
 
 ## 30-Minute Federated Learning Tutorial
 
-[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/examples/simulation_pytorch_colab/tutorial.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/examples/simulation_pytorch_colab/tutorial.ipynb))
+[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/examples/simulation-pytorch-colab/tutorial.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/examples/simulation-pytorch-colab/tutorial.ipynb))
 
 
 ## Documentation
 
 [Flower Docs](https://flower.dev/docs):
 * [Installation](https://flower.dev/docs/framework/installation.html)
 * [Quickstart (TensorFlow)](https://flower.dev/framework/docs/quickstart-tensorflow.html)
```

#### html2text {}

```diff
@@ -55,84 +55,83 @@
 source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the
 [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/
 tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb)) Stay tuned, more
 tutorials are coming soon. Topics include **Privacy and Security in Federated
 Learning**, and **Scaling Federated Learning**. ## 30-Minute Federated Learning
 Tutorial [![Open in Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/
-examples/simulation_pytorch_colab/tutorial.ipynb) (or open the [Jupyter
-Notebook](https://github.com/adap/flower/blob/main/examples/
-simulation_pytorch_colab/tutorial.ipynb)) ## Documentation [Flower Docs](https:
-//flower.dev/docs): * [Installation](https://flower.dev/docs/framework/
-installation.html) * [Quickstart (TensorFlow)](https://flower.dev/framework/
-docs/quickstart-tensorflow.html) * [Quickstart (PyTorch)](https://flower.dev/
-docs/framework/quickstart-pytorch.html) * [Quickstart (Hugging Face)](https://
-flower.dev/docs/framework/quickstart-huggingface.html) * [Quickstart (PyTorch
-Lightning [code example])](https://flower.dev/docs/framework/quickstart-
-pytorch-lightning.html) * [Quickstart (MXNet)](https://flower.dev/docs/
-framework/example-mxnet-walk-through.html) * [Quickstart (Pandas)](https://
-flower.dev/docs/framework/quickstart-pandas.html) * [Quickstart (fastai)]
-(https://flower.dev/docs/framework/quickstart-fastai.html) * [Quickstart (JAX)]
-(https://flower.dev/docs/framework/quickstart-jax.html) * [Quickstart (scikit-
-learn)](https://flower.dev/docs/framework/quickstart-scikitlearn.html) *
-[Quickstart (Android [TFLite])](https://flower.dev/docs/framework/quickstart-
-android.html) * [Quickstart (iOS [CoreML])](https://flower.dev/docs/framework/
-quickstart-ios.html) ## Flower Baselines Flower Baselines is a collection of
-community-contributed experiments that reproduce the experiments performed in
-popular federated learning publications. Researchers can build on Flower
-Baselines to quickly evaluate new ideas: * [FedAvg](https://arxiv.org/abs/
-1602.05629): * [MNIST](https://github.com/adap/flower/tree/main/baselines/
-flwr_baselines/flwr_baselines/publications/fedavg_mnist) * [FedProx](https://
-arxiv.org/abs/1812.06127): * [MNIST](https://github.com/adap/flower/tree/main/
-baselines/fedprox/) * [FedBN: Federated Learning on non-IID Features via Local
-Batch Normalization](https://arxiv.org/abs/2102.07623): * [Convergence Rate]
-(https://github.com/adap/flower/tree/main/baselines/flwr_baselines/
-flwr_baselines/publications/fedbn/convergence_rate) * [Adaptive Federated
-Optimization](https://arxiv.org/abs/2003.00295): * [CIFAR-10/100](https://
+examples/simulation-pytorch-colab/tutorial.ipynb) (or open the [Jupyter
+Notebook](https://github.com/adap/flower/blob/main/examples/simulation-pytorch-
+colab/tutorial.ipynb)) ## Documentation [Flower Docs](https://flower.dev/docs):
+* [Installation](https://flower.dev/docs/framework/installation.html) *
+[Quickstart (TensorFlow)](https://flower.dev/framework/docs/quickstart-
+tensorflow.html) * [Quickstart (PyTorch)](https://flower.dev/docs/framework/
+quickstart-pytorch.html) * [Quickstart (Hugging Face)](https://flower.dev/docs/
+framework/quickstart-huggingface.html) * [Quickstart (PyTorch Lightning [code
+example])](https://flower.dev/docs/framework/quickstart-pytorch-lightning.html)
+* [Quickstart (MXNet)](https://flower.dev/docs/framework/example-mxnet-walk-
+through.html) * [Quickstart (Pandas)](https://flower.dev/docs/framework/
+quickstart-pandas.html) * [Quickstart (fastai)](https://flower.dev/docs/
+framework/quickstart-fastai.html) * [Quickstart (JAX)](https://flower.dev/docs/
+framework/quickstart-jax.html) * [Quickstart (scikit-learn)](https://
+flower.dev/docs/framework/quickstart-scikitlearn.html) * [Quickstart (Android
+[TFLite])](https://flower.dev/docs/framework/quickstart-android.html) *
+[Quickstart (iOS [CoreML])](https://flower.dev/docs/framework/quickstart-
+ios.html) ## Flower Baselines Flower Baselines is a collection of community-
+contributed experiments that reproduce the experiments performed in popular
+federated learning publications. Researchers can build on Flower Baselines to
+quickly evaluate new ideas: * [FedAvg](https://arxiv.org/abs/1602.05629): *
+[MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/
+flwr_baselines/publications/fedavg_mnist) * [FedProx](https://arxiv.org/abs/
+1812.06127): * [MNIST](https://github.com/adap/flower/tree/main/baselines/
+fedprox/) * [FedBN: Federated Learning on non-IID Features via Local Batch
+Normalization](https://arxiv.org/abs/2102.07623): * [Convergence Rate](https://
 github.com/adap/flower/tree/main/baselines/flwr_baselines/flwr_baselines/
-publications/adaptive_federated_optimization) Check the Flower documentation to
-learn more: [Using Baselines](https://flower.dev/docs/baselines/using-
-baselines.html) The Flower community loves contributions! Make your work more
-visible and enable others to build on it by contributing it as a baseline:
-[Contributing Baselines](https://flower.dev/docs/baselines/contributing-
-baselines.html) ## Flower Usage Examples Several code examples show different
-usage scenarios of Flower (in combination with popular machine learning
-frameworks such as PyTorch or TensorFlow). Quickstart examples: * [Quickstart
-(TensorFlow)](https://github.com/adap/flower/tree/main/examples/quickstart-
-tensorflow) * [Quickstart (PyTorch)](https://github.com/adap/flower/tree/main/
-examples/quickstart-pytorch) * [Quickstart (Hugging Face)](https://github.com/
-adap/flower/tree/main/examples/quickstart-huggingface) * [Quickstart (PyTorch
-Lightning)](https://github.com/adap/flower/tree/main/examples/quickstart-
-pytorch-lightning) * [Quickstart (fastai)](https://github.com/adap/flower/tree/
-main/examples/quickstart-fastai) * [Quickstart (Pandas)](https://github.com/
-adap/flower/tree/main/examples/quickstart-pandas) * [Quickstart (MXNet)](https:
-//github.com/adap/flower/tree/main/examples/quickstart-mxnet) * [Quickstart
-(JAX)](https://github.com/adap/flower/tree/main/examples/quickstart-jax) *
-[Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/
-sklearn-logreg-mnist) * [Quickstart (Android [TFLite])](https://github.com/
-adap/flower/tree/main/examples/android) * [Quickstart (iOS [CoreML])](https://
-github.com/adap/flower/tree/main/examples/ios) Other [examples](https://
-github.com/adap/flower/tree/main/examples): * [Raspberry Pi & Nvidia Jetson
-Tutorial](https://github.com/adap/flower/tree/main/examples/embedded-devices) *
-[PyTorch: From Centralized to Federated](https://github.com/adap/flower/tree/
-main/examples/pytorch-from-centralized-to-federated) * [MXNet: From Centralized
-to Federated](https://github.com/adap/flower/tree/main/examples/mxnet-from-
-centralized-to-federated) * [Advanced Flower with TensorFlow/Keras](https://
-github.com/adap/flower/tree/main/examples/advanced-tensorflow) * [Advanced
-Flower with PyTorch](https://github.com/adap/flower/tree/main/examples/
-advanced-pytorch) * Single-Machine Simulation of Federated Learning Systems (
-[PyTorch](https://github.com/adap/flower/tree/main/examples/
-simulation_pytorch)) ([Tensorflow](https://github.com/adap/flower/tree/main/
-examples/simulation_tensorflow)) ## Community Flower is built by a wonderful
-community of researchers and engineers. [Join Slack](https://flower.dev/join-
-slack) to meet them, [contributions](#contributing-to-flower) are welcome.
-[https://contrib.rocks/image?repo=adap/flower] ## Citation If you publish work
-that uses Flower, please cite Flower as follows: ```bibtex @article
-{beutel2020flower, title={Flower: A Friendly Federated Learning Research
-Framework}, author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and
-Qiu, Xinchi and Fernandez-Marques, Javier and Gao, Yan and Sani, Lorenzo and
-Kwing, Hei Li and Parcollet, Titouan and GusmÃ£o, Pedro PB de and Lane,
-Nicholas D}, journal={arXiv preprint arXiv:2007.14390}, year={2020} } ```
-Please also consider adding your publication to the list of Flower-based
-publications in the docs, just open a Pull Request. ## Contributing to Flower
-We welcome contributions. Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get
-started!
+publications/fedbn/convergence_rate) * [Adaptive Federated Optimization](https:
+//arxiv.org/abs/2003.00295): * [CIFAR-10/100](https://github.com/adap/flower/
+tree/main/baselines/flwr_baselines/flwr_baselines/publications/
+adaptive_federated_optimization) Check the Flower documentation to learn more:
+[Using Baselines](https://flower.dev/docs/baselines/using-baselines.html) The
+Flower community loves contributions! Make your work more visible and enable
+others to build on it by contributing it as a baseline: [Contributing
+Baselines](https://flower.dev/docs/baselines/contributing-baselines.html) ##
+Flower Usage Examples Several code examples show different usage scenarios of
+Flower (in combination with popular machine learning frameworks such as PyTorch
+or TensorFlow). Quickstart examples: * [Quickstart (TensorFlow)](https://
+github.com/adap/flower/tree/main/examples/quickstart-tensorflow) * [Quickstart
+(PyTorch)](https://github.com/adap/flower/tree/main/examples/quickstart-
+pytorch) * [Quickstart (Hugging Face)](https://github.com/adap/flower/tree/
+main/examples/quickstart-huggingface) * [Quickstart (PyTorch Lightning)](https:
+//github.com/adap/flower/tree/main/examples/quickstart-pytorch-lightning) *
+[Quickstart (fastai)](https://github.com/adap/flower/tree/main/examples/
+quickstart-fastai) * [Quickstart (Pandas)](https://github.com/adap/flower/tree/
+main/examples/quickstart-pandas) * [Quickstart (MXNet)](https://github.com/
+adap/flower/tree/main/examples/quickstart-mxnet) * [Quickstart (JAX)](https://
+github.com/adap/flower/tree/main/examples/quickstart-jax) * [Quickstart
+(scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-
+logreg-mnist) * [Quickstart (Android [TFLite])](https://github.com/adap/flower/
+tree/main/examples/android) * [Quickstart (iOS [CoreML])](https://github.com/
+adap/flower/tree/main/examples/ios) Other [examples](https://github.com/adap/
+flower/tree/main/examples): * [Raspberry Pi & Nvidia Jetson Tutorial](https://
+github.com/adap/flower/tree/main/examples/embedded-devices) * [PyTorch: From
+Centralized to Federated](https://github.com/adap/flower/tree/main/examples/
+pytorch-from-centralized-to-federated) * [MXNet: From Centralized to Federated]
+(https://github.com/adap/flower/tree/main/examples/mxnet-from-centralized-to-
+federated) * [Advanced Flower with TensorFlow/Keras](https://github.com/adap/
+flower/tree/main/examples/advanced-tensorflow) * [Advanced Flower with PyTorch]
+(https://github.com/adap/flower/tree/main/examples/advanced-pytorch) * Single-
+Machine Simulation of Federated Learning Systems ([PyTorch](https://github.com/
+adap/flower/tree/main/examples/simulation_pytorch)) ([Tensorflow](https://
+github.com/adap/flower/tree/main/examples/simulation_tensorflow)) ## Community
+Flower is built by a wonderful community of researchers and engineers. [Join
+Slack](https://flower.dev/join-slack) to meet them, [contributions]
+(#contributing-to-flower) are welcome. [https://contrib.rocks/image?repo=adap/
+flower] ## Citation If you publish work that uses Flower, please cite Flower as
+follows: ```bibtex @article{beutel2020flower, title={Flower: A Friendly
+Federated Learning Research Framework}, author={Beutel, Daniel J and Topal,
+Taner and Mathur, Akhil and Qiu, Xinchi and Fernandez-Marques, Javier and Gao,
+Yan and Sani, Lorenzo and Kwing, Hei Li and Parcollet, Titouan and GusmÃ£o,
+Pedro PB de and Lane, Nicholas D}, journal={arXiv preprint arXiv:2007.14390},
+year={2020} } ``` Please also consider adding your publication to the list of
+Flower-based publications in the docs, just open a Pull Request. ##
+Contributing to Flower We welcome contributions. Please see [CONTRIBUTING.md]
+(CONTRIBUTING.md) to get started!
```

### Comparing `flwr_nightly-1.5.0.dev20230719/pyproject.toml` & `flwr_nightly-1.5.0.dev20230720/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.5.0-dev20230719"
+version = "1.5.0-dev20230720"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.dev>"]
 readme = "README.md"
 homepage = "https://flower.dev"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.dev"
@@ -59,14 +59,16 @@
 
 [tool.poetry.dependencies]
 python = "^3.7"
 # Mandatory dependencies
 numpy = "^1.21.0"
 grpcio = "^1.48.2,!=1.52.0"
 protobuf = "^3.19.0"
+cryptography = "^41.0.2"
+pycryptodome = "^3.18.0"
 importlib-metadata = { version = "^4.0.0", markers = "python_version < '3.8'" }
 iterators = "^0.0.2"
 # Optional dependencies (VCE)
 ray = { version = "==2.5.1", extras = ["default"], optional = true }
 pydantic = { version = "<2.0.0", optional = true }
 # Optional dependencies (REST transport layer)
 requests = { version = "^2.28.2", optional = true }
```

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/__init__.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/__init__.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/app.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/client.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/client/rest_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/__init__.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/address.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/constant.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/date.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/dp.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/grpc.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/logger.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/parameter.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/serde.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/serde.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """ProtoBuf serialization and deserialization."""
 
 
-from typing import Any, List, cast
+from typing import Any, Dict, List, cast
 
+from flwr.proto.task_pb2 import Value
 from flwr.proto.transport_pb2 import (
     ClientMessage,
     Code,
     Parameters,
     Reason,
     Scalar,
     ServerMessage,
@@ -479,7 +480,91 @@
 
 
 def scalar_from_proto(scalar_msg: Scalar) -> typing.Scalar:
     """Deserialize `Scalar` from ProtoBuf."""
     scalar_field = scalar_msg.WhichOneof("scalar")
     scalar = getattr(scalar_msg, cast(str, scalar_field))
     return cast(typing.Scalar, scalar)
+
+
+# === Value messages ===
+
+
+_python_type_to_field_name = {
+    float: "double",
+    int: "sint64",
+    bool: "bool",
+    str: "string",
+    bytes: "bytes",
+}
+
+
+_python_list_type_to_message_and_field_name = {
+    float: (Value.DoubleList, "double_list"),
+    int: (Value.Sint64List, "sint64_list"),
+    bool: (Value.BoolList, "bool_list"),
+    str: (Value.StringList, "string_list"),
+    bytes: (Value.BytesList, "bytes_list"),
+}
+
+
+def _check_value(value: typing.Value) -> None:
+    if isinstance(value, tuple(_python_type_to_field_name.keys())):
+        return
+    if isinstance(value, list) and isinstance(
+        value[0], tuple(_python_type_to_field_name.keys())
+    ):
+        data_type = type(value[0])
+        for element in value:
+            if isinstance(element, data_type):
+                continue
+            raise Exception(
+                f"Inconsistent type: the types of elements in the list must be the same"
+                f"(expected {data_type}, but got {type(element)})"
+            )
+    else:
+        raise TypeError(
+            f"Accepted types: {bool, bytes, float, int, str} or "
+            f"list of these types."
+        )
+
+
+def value_to_proto(value: typing.Value) -> Value:
+    """Serialize `Value` to ProtoBuf."""
+    _check_value(value)
+
+    arg = {}
+    if isinstance(value, list):
+        msg_class, field_name = _python_list_type_to_message_and_field_name[
+            type(value[0])
+        ]
+        arg[field_name] = msg_class(vals=value)
+    else:
+        arg[_python_type_to_field_name[type(value)]] = value
+    return Value(**arg)
+
+
+def value_from_proto(value_msg: Value) -> typing.Value:
+    """Deserialize `Value` from ProtoBuf."""
+    value_field = cast(str, value_msg.WhichOneof("value"))
+    if value_field.endswith("list"):
+        value = list(getattr(value_msg, value_field).vals)
+    else:
+        value = getattr(value_msg, value_field)
+    return cast(typing.Value, value)
+
+
+# === Named Values ===
+
+
+def named_values_to_proto(
+    named_values: Dict[str, typing.Value],
+) -> Dict[str, Value]:
+    """Serialize named values to ProtoBuf."""
+    return {name: value_to_proto(value) for name, value in named_values.items()}
+
+
+def named_values_from_proto(
+    named_values_proto: Dict[str, Value]
+) -> Dict[str, typing.Value]:
+    """Deserialize named values from ProtoBuf."""
+    return {name: value_from_proto(value) for name, value in named_values_proto.items()}
```

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/typing.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/typing.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,26 @@
 NDArrays = List[NDArray]
 
 # The following union type contains Python types corresponding to ProtoBuf types that
 # ProtoBuf considers to be "Scalar Value Types", even though some of them arguably do
 # not conform to other definitions of what a scalar is. Source:
 # https://developers.google.com/protocol-buffers/docs/overview#scalar
 Scalar = Union[bool, bytes, float, int, str]
+Value = Union[
+    bool,
+    bytes,
+    float,
+    int,
+    str,
+    List[bool],
+    List[bytes],
+    List[float],
+    List[int],
+    List[str],
+]
 
 Metrics = Dict[str, Scalar]
 MetricsAggregationFn = Callable[[List[Tuple[int, Metrics]]], Metrics]
 
 Config = Dict[str, Scalar]
 Properties = Dict[str, Scalar]
```

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/common/version.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/driver/app.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/driver/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/driver/driver.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/driver/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/driver/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/driver/driver_client_proxy.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/driver/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/__init__.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/app.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/criterion.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/driver/driver_servicer.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/__init__.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/rest_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/history.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/server.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/state/__init__.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/state/in_memory_state.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/state/sqlite_state.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/state/state.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/state/state_factory.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/server/utils/validator.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 from typing import List, Union
 
 from flwr.proto.task_pb2 import TaskIns, TaskRes
 
 
-# pylint: disable-next=too-many-branches
+# pylint: disable-next=too-many-branches,too-many-statements
 def validate_task_ins_or_res(tasks_ins_res: Union[TaskIns, TaskRes]) -> List[str]:
     """Validate a TaskIns or TaskRes."""
     validation_errors = []
 
     if tasks_ins_res.task_id != "":
         validation_errors.append("non-empty `task_id`")
 
@@ -59,20 +59,29 @@
             validation_errors.append("anonymous consumers MUST NOT set a `node_id`")
         if (
             not tasks_ins_res.task.consumer.anonymous
             and tasks_ins_res.task.consumer.node_id == 0
         ):
             validation_errors.append("non-anonymous consumer MUST provide a `node_id`")
 
-        # Legacy ServerMessage
-        if not tasks_ins_res.task.HasField("legacy_server_message"):
+        # Content check
+        has_fields = {
+            "sa": tasks_ins_res.task.HasField("sa"),
+            "legacy_server_message": tasks_ins_res.task.HasField(
+                "legacy_server_message"
+            ),
+        }
+        if not (has_fields["sa"] or has_fields["legacy_server_message"]):
+            err_msg = ", ".join([f"`{field}`" for field in has_fields])
             validation_errors.append(
-                "`task` does not set field `legacy_server_message`"
+                f"`task` in `TaskIns` must set at least one of fields {{{err_msg}}}"
             )
-        if not tasks_ins_res.task.legacy_server_message.HasField("msg"):
+        if has_fields[
+            "legacy_server_message"
+        ] and not tasks_ins_res.task.legacy_server_message.HasField("msg"):
             validation_errors.append("`legacy_server_message` does not set field `msg`")
 
         # Ancestors
         if len(tasks_ins_res.task.ancestry) != 0:
             validation_errors.append("`ancestry` is not empty")
 
     # TaskRes specific
@@ -101,20 +110,29 @@
             validation_errors.append("anonymous consumers MUST NOT set a `node_id`")
         if (
             not tasks_ins_res.task.consumer.anonymous
             and tasks_ins_res.task.consumer.node_id == 0
         ):
             validation_errors.append("non-anonymous consumer MUST provide a `node_id`")
 
-        # Legacy ClientMessage
-        if not tasks_ins_res.task.HasField("legacy_client_message"):
+        # Content check
+        has_fields = {
+            "sa": tasks_ins_res.task.HasField("sa"),
+            "legacy_client_message": tasks_ins_res.task.HasField(
+                "legacy_client_message"
+            ),
+        }
+        if not (has_fields["sa"] or has_fields["legacy_client_message"]):
+            err_msg = ", ".join([f"`{field}`" for field in has_fields])
             validation_errors.append(
-                "`task` does not set field `legacy_client_message`"
+                f"`task` in `TaskRes` must set at least one of fields {{{err_msg}}}"
             )
-        if not tasks_ins_res.task.legacy_client_message.HasField("msg"):
+        if has_fields[
+            "legacy_client_message"
+        ] and not tasks_ins_res.task.legacy_client_message.HasField("msg"):
             validation_errors.append("`legacy_client_message` does not set field `msg`")
 
         # Ancestors
         if len(tasks_ins_res.task.ancestry) == 0:
             validation_errors.append("`ancestry` is empty")
 
     return validation_errors
```

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/simulation/app.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.5.0.dev20230720/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230719/PKG-INFO` & `flwr_nightly-1.5.0.dev20230720/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.5.0.dev20230719
+Version: 1.5.0.dev20230720
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.dev
 License: Apache-2.0
 Keywords: flower,fl,federated learning,federated analytics,federated evaluation,machine learning
 Author: The Flower Authors
 Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0
@@ -28,20 +28,22 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Provides-Extra: rest
 Provides-Extra: simulation
+Requires-Dist: cryptography (>=41.0.2,<42.0.0)
 Requires-Dist: fastapi (>=0.95.0,<0.96.0) ; extra == "rest"
 Requires-Dist: grpcio (>=1.48.2,<2.0.0,!=1.52.0)
 Requires-Dist: importlib-metadata (>=4.0.0,<5.0.0) ; python_version < "3.8"
 Requires-Dist: iterators (>=0.0.2,<0.0.3)
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
 Requires-Dist: protobuf (>=3.19.0,<4.0.0)
+Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
 Requires-Dist: pydantic (<2.0.0) ; extra == "simulation"
 Requires-Dist: ray[default] (==2.5.1) ; extra == "simulation"
 Requires-Dist: requests (>=2.28.2,<3.0.0) ; extra == "rest"
 Requires-Dist: starlette (>=0.27.0,<0.28.0) ; extra == "rest"
 Requires-Dist: uvicorn[standard] (>=0.21.1,<0.22.0) ; extra == "rest"
 Project-URL: Documentation, https://flower.dev
 Project-URL: Repository, https://github.com/adap/flower
@@ -116,15 +118,15 @@
 
    [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb))
 
 Stay tuned, more tutorials are coming soon. Topics include **Privacy and Security in Federated Learning**, and **Scaling Federated Learning**.
 
 ## 30-Minute Federated Learning Tutorial
 
-[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/examples/simulation_pytorch_colab/tutorial.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/examples/simulation_pytorch_colab/tutorial.ipynb))
+[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/examples/simulation-pytorch-colab/tutorial.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/examples/simulation-pytorch-colab/tutorial.ipynb))
 
 
 ## Documentation
 
 [Flower Docs](https://flower.dev/docs):
 * [Installation](https://flower.dev/docs/framework/installation.html)
 * [Quickstart (TensorFlow)](https://flower.dev/framework/docs/quickstart-tensorflow.html)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.5.0.dev20230719 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.5.0.dev20230720 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.dev
 License: Apache-2.0 Keywords: flower,fl,federated learning,federated
 analytics,federated evaluation,machine learning Author: The Flower Authors
 Author-email: hello@flower.dev Requires-Python: >=3.7,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
@@ -14,26 +14,27 @@
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
 Only Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Scientific/
 Engineering :: Mathematics Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: Typing :: Typed
-Provides-Extra: rest Provides-Extra: simulation Requires-Dist: fastapi
-(>=0.95.0,<0.96.0) ; extra == "rest" Requires-Dist: grpcio
-(>=1.48.2,<2.0.0,!=1.52.0) Requires-Dist: importlib-metadata (>=4.0.0,<5.0.0) ;
-python_version < "3.8" Requires-Dist: iterators (>=0.0.2,<0.0.3) Requires-Dist:
-numpy (>=1.21.0,<2.0.0) Requires-Dist: protobuf (>=3.19.0,<4.0.0) Requires-
-Dist: pydantic (<2.0.0) ; extra == "simulation" Requires-Dist: ray[default]
-(==2.5.1) ; extra == "simulation" Requires-Dist: requests (>=2.28.2,<3.0.0) ;
-extra == "rest" Requires-Dist: starlette (>=0.27.0,<0.28.0) ; extra == "rest"
-Requires-Dist: uvicorn[standard] (>=0.21.1,<0.22.0) ; extra == "rest" Project-
-URL: Documentation, https://flower.dev Project-URL: Repository, https://
-github.com/adap/flower Description-Content-Type: text/markdown # Flower: A
-Friendly Federated Learning Framework
+Provides-Extra: rest Provides-Extra: simulation Requires-Dist: cryptography
+(>=41.0.2,<42.0.0) Requires-Dist: fastapi (>=0.95.0,<0.96.0) ; extra == "rest"
+Requires-Dist: grpcio (>=1.48.2,<2.0.0,!=1.52.0) Requires-Dist: importlib-
+metadata (>=4.0.0,<5.0.0) ; python_version < "3.8" Requires-Dist: iterators
+(>=0.0.2,<0.0.3) Requires-Dist: numpy (>=1.21.0,<2.0.0) Requires-Dist: protobuf
+(>=3.19.0,<4.0.0) Requires-Dist: pycryptodome (>=3.18.0,<4.0.0) Requires-Dist:
+pydantic (<2.0.0) ; extra == "simulation" Requires-Dist: ray[default] (==2.5.1)
+; extra == "simulation" Requires-Dist: requests (>=2.28.2,<3.0.0) ; extra ==
+"rest" Requires-Dist: starlette (>=0.27.0,<0.28.0) ; extra == "rest" Requires-
+Dist: uvicorn[standard] (>=0.21.1,<0.22.0) ; extra == "rest" Project-URL:
+Documentation, https://flower.dev Project-URL: Repository, https://github.com/
+adap/flower Description-Content-Type: text/markdown # Flower: A Friendly
+Federated Learning Framework
                                [Flower_Website]
                   Website | Blog | Docs | Conference | Slack
 
 [![GitHub license](https://img.shields.io/github/license/adap/flower)](https://
 github.com/adap/flower/blob/main/LICENSE) [![PRs Welcome](https://
 img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/
 flower/blob/main/CONTRIBUTING.md) ![Build](https://github.com/adap/flower/
@@ -86,84 +87,83 @@
 source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the
 [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/
 tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb)) Stay tuned, more
 tutorials are coming soon. Topics include **Privacy and Security in Federated
 Learning**, and **Scaling Federated Learning**. ## 30-Minute Federated Learning
 Tutorial [![Open in Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/
-examples/simulation_pytorch_colab/tutorial.ipynb) (or open the [Jupyter
-Notebook](https://github.com/adap/flower/blob/main/examples/
-simulation_pytorch_colab/tutorial.ipynb)) ## Documentation [Flower Docs](https:
-//flower.dev/docs): * [Installation](https://flower.dev/docs/framework/
-installation.html) * [Quickstart (TensorFlow)](https://flower.dev/framework/
-docs/quickstart-tensorflow.html) * [Quickstart (PyTorch)](https://flower.dev/
-docs/framework/quickstart-pytorch.html) * [Quickstart (Hugging Face)](https://
-flower.dev/docs/framework/quickstart-huggingface.html) * [Quickstart (PyTorch
-Lightning [code example])](https://flower.dev/docs/framework/quickstart-
-pytorch-lightning.html) * [Quickstart (MXNet)](https://flower.dev/docs/
-framework/example-mxnet-walk-through.html) * [Quickstart (Pandas)](https://
-flower.dev/docs/framework/quickstart-pandas.html) * [Quickstart (fastai)]
-(https://flower.dev/docs/framework/quickstart-fastai.html) * [Quickstart (JAX)]
-(https://flower.dev/docs/framework/quickstart-jax.html) * [Quickstart (scikit-
-learn)](https://flower.dev/docs/framework/quickstart-scikitlearn.html) *
-[Quickstart (Android [TFLite])](https://flower.dev/docs/framework/quickstart-
-android.html) * [Quickstart (iOS [CoreML])](https://flower.dev/docs/framework/
-quickstart-ios.html) ## Flower Baselines Flower Baselines is a collection of
-community-contributed experiments that reproduce the experiments performed in
-popular federated learning publications. Researchers can build on Flower
-Baselines to quickly evaluate new ideas: * [FedAvg](https://arxiv.org/abs/
-1602.05629): * [MNIST](https://github.com/adap/flower/tree/main/baselines/
-flwr_baselines/flwr_baselines/publications/fedavg_mnist) * [FedProx](https://
-arxiv.org/abs/1812.06127): * [MNIST](https://github.com/adap/flower/tree/main/
-baselines/fedprox/) * [FedBN: Federated Learning on non-IID Features via Local
-Batch Normalization](https://arxiv.org/abs/2102.07623): * [Convergence Rate]
-(https://github.com/adap/flower/tree/main/baselines/flwr_baselines/
-flwr_baselines/publications/fedbn/convergence_rate) * [Adaptive Federated
-Optimization](https://arxiv.org/abs/2003.00295): * [CIFAR-10/100](https://
+examples/simulation-pytorch-colab/tutorial.ipynb) (or open the [Jupyter
+Notebook](https://github.com/adap/flower/blob/main/examples/simulation-pytorch-
+colab/tutorial.ipynb)) ## Documentation [Flower Docs](https://flower.dev/docs):
+* [Installation](https://flower.dev/docs/framework/installation.html) *
+[Quickstart (TensorFlow)](https://flower.dev/framework/docs/quickstart-
+tensorflow.html) * [Quickstart (PyTorch)](https://flower.dev/docs/framework/
+quickstart-pytorch.html) * [Quickstart (Hugging Face)](https://flower.dev/docs/
+framework/quickstart-huggingface.html) * [Quickstart (PyTorch Lightning [code
+example])](https://flower.dev/docs/framework/quickstart-pytorch-lightning.html)
+* [Quickstart (MXNet)](https://flower.dev/docs/framework/example-mxnet-walk-
+through.html) * [Quickstart (Pandas)](https://flower.dev/docs/framework/
+quickstart-pandas.html) * [Quickstart (fastai)](https://flower.dev/docs/
+framework/quickstart-fastai.html) * [Quickstart (JAX)](https://flower.dev/docs/
+framework/quickstart-jax.html) * [Quickstart (scikit-learn)](https://
+flower.dev/docs/framework/quickstart-scikitlearn.html) * [Quickstart (Android
+[TFLite])](https://flower.dev/docs/framework/quickstart-android.html) *
+[Quickstart (iOS [CoreML])](https://flower.dev/docs/framework/quickstart-
+ios.html) ## Flower Baselines Flower Baselines is a collection of community-
+contributed experiments that reproduce the experiments performed in popular
+federated learning publications. Researchers can build on Flower Baselines to
+quickly evaluate new ideas: * [FedAvg](https://arxiv.org/abs/1602.05629): *
+[MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/
+flwr_baselines/publications/fedavg_mnist) * [FedProx](https://arxiv.org/abs/
+1812.06127): * [MNIST](https://github.com/adap/flower/tree/main/baselines/
+fedprox/) * [FedBN: Federated Learning on non-IID Features via Local Batch
+Normalization](https://arxiv.org/abs/2102.07623): * [Convergence Rate](https://
 github.com/adap/flower/tree/main/baselines/flwr_baselines/flwr_baselines/
-publications/adaptive_federated_optimization) Check the Flower documentation to
-learn more: [Using Baselines](https://flower.dev/docs/baselines/using-
-baselines.html) The Flower community loves contributions! Make your work more
-visible and enable others to build on it by contributing it as a baseline:
-[Contributing Baselines](https://flower.dev/docs/baselines/contributing-
-baselines.html) ## Flower Usage Examples Several code examples show different
-usage scenarios of Flower (in combination with popular machine learning
-frameworks such as PyTorch or TensorFlow). Quickstart examples: * [Quickstart
-(TensorFlow)](https://github.com/adap/flower/tree/main/examples/quickstart-
-tensorflow) * [Quickstart (PyTorch)](https://github.com/adap/flower/tree/main/
-examples/quickstart-pytorch) * [Quickstart (Hugging Face)](https://github.com/
-adap/flower/tree/main/examples/quickstart-huggingface) * [Quickstart (PyTorch
-Lightning)](https://github.com/adap/flower/tree/main/examples/quickstart-
-pytorch-lightning) * [Quickstart (fastai)](https://github.com/adap/flower/tree/
-main/examples/quickstart-fastai) * [Quickstart (Pandas)](https://github.com/
-adap/flower/tree/main/examples/quickstart-pandas) * [Quickstart (MXNet)](https:
-//github.com/adap/flower/tree/main/examples/quickstart-mxnet) * [Quickstart
-(JAX)](https://github.com/adap/flower/tree/main/examples/quickstart-jax) *
-[Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/
-sklearn-logreg-mnist) * [Quickstart (Android [TFLite])](https://github.com/
-adap/flower/tree/main/examples/android) * [Quickstart (iOS [CoreML])](https://
-github.com/adap/flower/tree/main/examples/ios) Other [examples](https://
-github.com/adap/flower/tree/main/examples): * [Raspberry Pi & Nvidia Jetson
-Tutorial](https://github.com/adap/flower/tree/main/examples/embedded-devices) *
-[PyTorch: From Centralized to Federated](https://github.com/adap/flower/tree/
-main/examples/pytorch-from-centralized-to-federated) * [MXNet: From Centralized
-to Federated](https://github.com/adap/flower/tree/main/examples/mxnet-from-
-centralized-to-federated) * [Advanced Flower with TensorFlow/Keras](https://
-github.com/adap/flower/tree/main/examples/advanced-tensorflow) * [Advanced
-Flower with PyTorch](https://github.com/adap/flower/tree/main/examples/
-advanced-pytorch) * Single-Machine Simulation of Federated Learning Systems (
-[PyTorch](https://github.com/adap/flower/tree/main/examples/
-simulation_pytorch)) ([Tensorflow](https://github.com/adap/flower/tree/main/
-examples/simulation_tensorflow)) ## Community Flower is built by a wonderful
-community of researchers and engineers. [Join Slack](https://flower.dev/join-
-slack) to meet them, [contributions](#contributing-to-flower) are welcome.
-[https://contrib.rocks/image?repo=adap/flower] ## Citation If you publish work
-that uses Flower, please cite Flower as follows: ```bibtex @article
-{beutel2020flower, title={Flower: A Friendly Federated Learning Research
-Framework}, author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and
-Qiu, Xinchi and Fernandez-Marques, Javier and Gao, Yan and Sani, Lorenzo and
-Kwing, Hei Li and Parcollet, Titouan and GusmÃ£o, Pedro PB de and Lane,
-Nicholas D}, journal={arXiv preprint arXiv:2007.14390}, year={2020} } ```
-Please also consider adding your publication to the list of Flower-based
-publications in the docs, just open a Pull Request. ## Contributing to Flower
-We welcome contributions. Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get
-started!
+publications/fedbn/convergence_rate) * [Adaptive Federated Optimization](https:
+//arxiv.org/abs/2003.00295): * [CIFAR-10/100](https://github.com/adap/flower/
+tree/main/baselines/flwr_baselines/flwr_baselines/publications/
+adaptive_federated_optimization) Check the Flower documentation to learn more:
+[Using Baselines](https://flower.dev/docs/baselines/using-baselines.html) The
+Flower community loves contributions! Make your work more visible and enable
+others to build on it by contributing it as a baseline: [Contributing
+Baselines](https://flower.dev/docs/baselines/contributing-baselines.html) ##
+Flower Usage Examples Several code examples show different usage scenarios of
+Flower (in combination with popular machine learning frameworks such as PyTorch
+or TensorFlow). Quickstart examples: * [Quickstart (TensorFlow)](https://
+github.com/adap/flower/tree/main/examples/quickstart-tensorflow) * [Quickstart
+(PyTorch)](https://github.com/adap/flower/tree/main/examples/quickstart-
+pytorch) * [Quickstart (Hugging Face)](https://github.com/adap/flower/tree/
+main/examples/quickstart-huggingface) * [Quickstart (PyTorch Lightning)](https:
+//github.com/adap/flower/tree/main/examples/quickstart-pytorch-lightning) *
+[Quickstart (fastai)](https://github.com/adap/flower/tree/main/examples/
+quickstart-fastai) * [Quickstart (Pandas)](https://github.com/adap/flower/tree/
+main/examples/quickstart-pandas) * [Quickstart (MXNet)](https://github.com/
+adap/flower/tree/main/examples/quickstart-mxnet) * [Quickstart (JAX)](https://
+github.com/adap/flower/tree/main/examples/quickstart-jax) * [Quickstart
+(scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-
+logreg-mnist) * [Quickstart (Android [TFLite])](https://github.com/adap/flower/
+tree/main/examples/android) * [Quickstart (iOS [CoreML])](https://github.com/
+adap/flower/tree/main/examples/ios) Other [examples](https://github.com/adap/
+flower/tree/main/examples): * [Raspberry Pi & Nvidia Jetson Tutorial](https://
+github.com/adap/flower/tree/main/examples/embedded-devices) * [PyTorch: From
+Centralized to Federated](https://github.com/adap/flower/tree/main/examples/
+pytorch-from-centralized-to-federated) * [MXNet: From Centralized to Federated]
+(https://github.com/adap/flower/tree/main/examples/mxnet-from-centralized-to-
+federated) * [Advanced Flower with TensorFlow/Keras](https://github.com/adap/
+flower/tree/main/examples/advanced-tensorflow) * [Advanced Flower with PyTorch]
+(https://github.com/adap/flower/tree/main/examples/advanced-pytorch) * Single-
+Machine Simulation of Federated Learning Systems ([PyTorch](https://github.com/
+adap/flower/tree/main/examples/simulation_pytorch)) ([Tensorflow](https://
+github.com/adap/flower/tree/main/examples/simulation_tensorflow)) ## Community
+Flower is built by a wonderful community of researchers and engineers. [Join
+Slack](https://flower.dev/join-slack) to meet them, [contributions]
+(#contributing-to-flower) are welcome. [https://contrib.rocks/image?repo=adap/
+flower] ## Citation If you publish work that uses Flower, please cite Flower as
+follows: ```bibtex @article{beutel2020flower, title={Flower: A Friendly
+Federated Learning Research Framework}, author={Beutel, Daniel J and Topal,
+Taner and Mathur, Akhil and Qiu, Xinchi and Fernandez-Marques, Javier and Gao,
+Yan and Sani, Lorenzo and Kwing, Hei Li and Parcollet, Titouan and GusmÃ£o,
+Pedro PB de and Lane, Nicholas D}, journal={arXiv preprint arXiv:2007.14390},
+year={2020} } ``` Please also consider adding your publication to the list of
+Flower-based publications in the docs, just open a Pull Request. ##
+Contributing to Flower We welcome contributions. Please see [CONTRIBUTING.md]
+(CONTRIBUTING.md) to get started!
```

