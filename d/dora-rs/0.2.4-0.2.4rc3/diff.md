# Comparing `tmp/dora_rs-0.2.4.tar.gz` & `tmp/dora_rs-0.2.4rc3.tar.gz`

## Comparing `dora_rs-0.2.4.tar` & `dora_rs-0.2.4rc3.tar`

### file list

```diff
@@ -1,53 +1,52 @@
--rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 dora_rs-0.2.4/local_dependencies/dora-metrics/Cargo.toml
--rw-r--r--   0     1001      123     1483 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-metrics/src/lib.rs
--rw-r--r--   0        0        0      844 1970-01-01 00:00:00.000000 dora_rs-0.2.4/local_dependencies/dora-node-api/Cargo.toml
--rw-r--r--   0     1001      123     2429 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-node-api/src/daemon_connection/mod.rs
--rw-r--r--   0     1001      123     2149 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-node-api/src/daemon_connection/tcp.rs
--rw-r--r--   0     1001      123     2251 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-node-api/src/event_stream/event.rs
--rw-r--r--   0     1001      123     1505 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-node-api/src/event_stream/merged.rs
--rw-r--r--   0     1001      123     7024 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-node-api/src/event_stream/mod.rs
--rw-r--r--   0     1001      123     9248 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-node-api/src/event_stream/thread.rs
--rw-r--r--   0     1001      123      681 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-node-api/src/lib.rs
--rw-r--r--   0     1001      123     3649 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-node-api/src/node/control_channel.rs
--rw-r--r--   0     1001      123     5795 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-node-api/src/node/drop_stream.rs
--rw-r--r--   0     1001      123    12692 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-node-api/src/node/mod.rs
--rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 dora_rs-0.2.4/local_dependencies/dora-runtime/Cargo.toml
--rw-r--r--   0     1001      123    13208 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-runtime/src/lib.rs
--rw-r--r--   0     1001      123     4296 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-runtime/src/operator/channel.rs
--rw-r--r--   0     1001      123     2568 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-runtime/src/operator/mod.rs
--rw-r--r--   0     1001      123    13052 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-runtime/src/operator/python.rs
--rw-r--r--   0     1001      123     9727 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-runtime/src/operator/shared_lib.rs
--rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 dora_rs-0.2.4/local_dependencies/dora-tracing/Cargo.toml
--rw-r--r--   0     1001      123     1620 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-tracing/src/lib.rs
--rw-r--r--   0     1001      123     2248 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-tracing/src/telemetry.rs
--rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 dora_rs-0.2.4/local_dependencies/shared-memory-server/Cargo.toml
--rw-r--r--   0     1001      123     3249 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/shared-memory-server/src/bin/bench.rs
--rw-r--r--   0     1001      123     7343 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/shared-memory-server/src/channel.rs
--rw-r--r--   0     1001      123     2019 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/shared-memory-server/src/lib.rs
--rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 dora_rs-0.2.4/local_dependencies/dora-message/Cargo.toml
--rw-r--r--   0     1001      123      360 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-message/build.rs
--rw-r--r--   0     1001      123      229 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-message/schema/message.capnp
--rw-r--r--   0     1001      123     3225 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-message/src/lib.rs
--rw-r--r--   0     1001      123     7447 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-message/src/message_capnp.rs
--rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 dora_rs-0.2.4/local_dependencies/dora-core/Cargo.toml
--rw-r--r--   0     1001      123     9127 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-core/src/config.rs
--rw-r--r--   0     1001      123      957 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-core/src/coordinator_messages.rs
--rw-r--r--   0     1001      123     6695 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-core/src/daemon_messages.rs
--rw-r--r--   0     1001      123     8998 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-core/src/descriptor/mod.rs
--rw-r--r--   0     1001      123     7001 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-core/src/descriptor/validate.rs
--rw-r--r--   0     1001      123     6705 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-core/src/descriptor/visualize.rs
--rw-r--r--   0     1001      123      974 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-core/src/lib.rs
--rw-r--r--   0     1001      123     2066 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-core/src/topics.rs
--rw-r--r--   0        0        0      405 1970-01-01 00:00:00.000000 dora_rs-0.2.4/local_dependencies/dora-operator-api-types/Cargo.toml
--rw-r--r--   0     1001      123     2396 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-operator-api-types/src/lib.rs
--rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 dora_rs-0.2.4/local_dependencies/dora-operator-api-python/Cargo.toml
--rw-r--r--   0     1001      123     5862 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-operator-api-python/src/lib.rs
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 dora_rs-0.2.4/local_dependencies/dora-download/Cargo.toml
--rw-r--r--   0     1001      123     1285 2023-07-21 13:15:32.000000 dora_rs-0.2.4/local_dependencies/dora-download/src/lib.rs
--rw-r--r--   0        0        0      946 1970-01-01 00:00:00.000000 dora_rs-0.2.4/Cargo.toml
--rw-r--r--   0     1001      123      204 2023-07-21 13:15:32.000000 dora_rs-0.2.4/README.md
--rw-r--r--   0     1001      123      514 2023-07-21 13:15:32.000000 dora_rs-0.2.4/dora/__init__.py
--rw-r--r--   0     1001      123      153 2023-07-21 13:15:32.000000 dora_rs-0.2.4/pyproject.toml
--rw-r--r--   0     1001      123     3399 2023-07-21 13:15:32.000000 dora_rs-0.2.4/src/lib.rs
--rw-r--r--   0     1001      123   142556 2023-07-21 13:15:32.000000 dora_rs-0.2.4/Cargo.lock
--rw-r--r--   0        0        0      429 1970-01-01 00:00:00.000000 dora_rs-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/local_dependencies/dora-tracing/Cargo.toml
+-rw-r--r--   0     1001      123     1620 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-tracing/src/lib.rs
+-rw-r--r--   0     1001      123     2248 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-tracing/src/telemetry.rs
+-rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/local_dependencies/shared-memory-server/Cargo.toml
+-rw-r--r--   0     1001      123     3249 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/shared-memory-server/src/bin/bench.rs
+-rw-r--r--   0     1001      123     7334 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/shared-memory-server/src/channel.rs
+-rw-r--r--   0     1001      123     2010 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/shared-memory-server/src/lib.rs
+-rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/local_dependencies/dora-node-api/Cargo.toml
+-rw-r--r--   0     1001      123     2429 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/daemon_connection/mod.rs
+-rw-r--r--   0     1001      123     2149 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/daemon_connection/tcp.rs
+-rw-r--r--   0     1001      123     2209 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/event_stream/event.rs
+-rw-r--r--   0     1001      123     7008 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/event_stream/mod.rs
+-rw-r--r--   0     1001      123     9248 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/event_stream/thread.rs
+-rw-r--r--   0     1001      123      673 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/lib.rs
+-rw-r--r--   0     1001      123     3649 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/node/control_channel.rs
+-rw-r--r--   0     1001      123     5795 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/node/drop_stream.rs
+-rw-r--r--   0     1001      123    12329 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/node/mod.rs
+-rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/local_dependencies/dora-runtime/Cargo.toml
+-rw-r--r--   0     1001      123    13208 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-runtime/src/lib.rs
+-rw-r--r--   0     1001      123     4296 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-runtime/src/operator/channel.rs
+-rw-r--r--   0     1001      123     2568 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-runtime/src/operator/mod.rs
+-rw-r--r--   0     1001      123    12634 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-runtime/src/operator/python.rs
+-rw-r--r--   0     1001      123     9727 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-runtime/src/operator/shared_lib.rs
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/local_dependencies/dora-metrics/Cargo.toml
+-rw-r--r--   0     1001      123     1483 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-metrics/src/lib.rs
+-rw-r--r--   0        0        0      409 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/local_dependencies/dora-operator-api-types/Cargo.toml
+-rw-r--r--   0     1001      123     2396 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-operator-api-types/src/lib.rs
+-rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/local_dependencies/dora-operator-api-python/Cargo.toml
+-rw-r--r--   0     1001      123     5862 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-operator-api-python/src/lib.rs
+-rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/local_dependencies/dora-core/Cargo.toml
+-rw-r--r--   0     1001      123     9127 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-core/src/config.rs
+-rw-r--r--   0     1001      123      957 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-core/src/coordinator_messages.rs
+-rw-r--r--   0     1001      123     6695 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-core/src/daemon_messages.rs
+-rw-r--r--   0     1001      123     8998 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-core/src/descriptor/mod.rs
+-rw-r--r--   0     1001      123     7001 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-core/src/descriptor/validate.rs
+-rw-r--r--   0     1001      123     6705 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-core/src/descriptor/visualize.rs
+-rw-r--r--   0     1001      123      974 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-core/src/lib.rs
+-rw-r--r--   0     1001      123     2066 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-core/src/topics.rs
+-rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/local_dependencies/dora-download/Cargo.toml
+-rw-r--r--   0     1001      123     1285 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-download/src/lib.rs
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/local_dependencies/dora-message/Cargo.toml
+-rw-r--r--   0     1001      123      360 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-message/build.rs
+-rw-r--r--   0     1001      123      229 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-message/schema/message.capnp
+-rw-r--r--   0     1001      123     3225 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-message/src/lib.rs
+-rw-r--r--   0     1001      123     7447 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-message/src/message_capnp.rs
+-rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/Cargo.toml
+-rw-r--r--   0     1001      123      204 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/README.md
+-rw-r--r--   0     1001      123      518 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/dora/__init__.py
+-rw-r--r--   0     1001      123      153 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/pyproject.toml
+-rw-r--r--   0     1001      123     3399 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/src/lib.rs
+-rw-r--r--   0     1001      123   142629 2023-07-18 10:52:39.000000 dora_rs-0.2.4rc3/Cargo.lock
+-rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/PKG-INFO
```

### Comparing `dora_rs-0.2.4/local_dependencies/dora-metrics/Cargo.toml` & `dora_rs-0.2.4rc3/local_dependencies/dora-metrics/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-metrics"
-version= "0.2.4"
+version= "0.2.4-rc3"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `dora_rs-0.2.4/local_dependencies/dora-metrics/src/lib.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-metrics/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-node-api/src/daemon_connection/mod.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/daemon_connection/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-node-api/src/daemon_connection/tcp.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/daemon_connection/tcp.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-node-api/src/event_stream/event.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/event_stream/event.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use std::{ptr::NonNull, sync::Arc};
 
 use dora_core::{
     config::{DataId, OperatorId},
     message::Metadata,
 };
 use eyre::Context;
-use shared_memory_extended::{Shmem, ShmemConf};
+use shared_memory::{Shmem, ShmemConf};
 
 #[derive(Debug)]
 #[non_exhaustive]
 pub enum Event {
     Stop,
     Reload {
         operator_id: Option<OperatorId>,
@@ -74,15 +74,14 @@
 }
 
 impl MappedInputData {
     pub(crate) unsafe fn map(shared_memory_id: &str, len: usize) -> eyre::Result<Self> {
         let memory = Box::new(
             ShmemConf::new()
                 .os_id(shared_memory_id)
-                .writable(false)
                 .open()
                 .wrap_err("failed to map shared memory input")?,
         );
         Ok(MappedInputData { memory, len })
     }
 }
```

### Comparing `dora_rs-0.2.4/local_dependencies/dora-node-api/src/event_stream/mod.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/event_stream/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
         self, DaemonCommunication, DaemonRequest, DataflowId, NodeEvent, Timestamped,
     },
     message::uhlc,
 };
 use eyre::{eyre, Context};
 
 mod event;
-pub mod merged;
 mod thread;
 
 pub struct EventStream {
     node_id: NodeId,
     receiver: flume::r#async::RecvStream<'static, EventItem>,
     _thread_handle: EventStreamThreadHandle,
     close_channel: DaemonChannel,
```

### Comparing `dora_rs-0.2.4/local_dependencies/dora-node-api/src/event_stream/thread.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/event_stream/thread.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-node-api/src/lib.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/lib.rs`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 //!
 //! ```bash
 //! dora new project_xyz --kind dataflow
 //! ```
 //!
 pub use dora_core;
 pub use dora_core::message::{uhlc, Metadata, MetadataParameters};
-pub use event_stream::{merged, Data, Event, EventStream, MappedInputData};
+pub use event_stream::{Data, Event, EventStream, MappedInputData};
 pub use flume::Receiver;
 pub use node::{DataSample, DoraNode};
 
 mod daemon_connection;
 mod event_stream;
 mod node;
```

### Comparing `dora_rs-0.2.4/local_dependencies/dora-node-api/src/node/control_channel.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/node/control_channel.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-node-api/src/node/drop_stream.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/node/drop_stream.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-node-api/src/node/mod.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/node/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 use dora_core::{
     config::{DataId, NodeId, NodeRunConfig},
     daemon_messages::{Data, DropToken, NodeConfig},
     descriptor::Descriptor,
     message::{uhlc, Metadata, MetadataParameters},
 };
 use eyre::{bail, WrapErr};
-use shared_memory_extended::{Shmem, ShmemConf};
+use shared_memory::{Shmem, ShmemConf};
 use std::{
     collections::{HashMap, VecDeque},
     ops::{Deref, DerefMut},
     sync::Arc,
     time::Duration,
 };
 
@@ -129,26 +129,14 @@
     {
         let mut sample = self.allocate_data_sample(data_len)?;
         data(&mut sample);
 
         self.send_output_sample(output_id, parameters, Some(sample))
     }
 
-    pub fn send_output_bytes(
-        &mut self,
-        output_id: DataId,
-        parameters: MetadataParameters,
-        data_len: usize,
-        data: &[u8],
-    ) -> eyre::Result<()> {
-        self.send_output(output_id, parameters, data_len, |sample| {
-            sample.copy_from_slice(data)
-        })
-    }
-
     pub fn send_output_sample(
         &mut self,
         output_id: DataId,
         parameters: MetadataParameters,
         sample: Option<DataSample>,
     ) -> eyre::Result<()> {
         self.handle_finished_drop_tokens()?;
@@ -227,15 +215,14 @@
             Some(i) => {
                 // we know that this index exists, so we can safely unwrap here
                 self.cache.remove(i).unwrap()
             }
             None => ShmemHandle(Box::new(
                 ShmemConf::new()
                     .size(data_len)
-                    .writable(true)
                     .create()
                     .wrap_err("failed to allocate shared memory")?,
             )),
         };
         assert!(memory.len() >= data_len);
 
         Ok(memory)
```

### Comparing `dora_rs-0.2.4/local_dependencies/dora-runtime/Cargo.toml` & `dora_rs-0.2.4rc3/local_dependencies/dora-runtime/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-runtime"
-version= "0.2.4"
+version= "0.2.4-rc3"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `dora_rs-0.2.4/local_dependencies/dora-runtime/src/lib.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-runtime/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-runtime/src/operator/channel.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-runtime/src/operator/channel.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-runtime/src/operator/mod.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-runtime/src/operator/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-runtime/src/operator/python.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-runtime/src/operator/python.rs`

 * *Files 6% similar despite different names*

```diff
@@ -271,19 +271,14 @@
 
     use super::SendOutputCallback;
     use dora_operator_api_python::{process_python_output, pydict_to_metadata, python_output_len};
     use eyre::{eyre, Context, Result};
     use pyo3::{pymethods, types::PyDict, PyObject, Python};
     use tokio::sync::oneshot;
 
-    /// Send an output from the operator:
-    /// - the first argument is the `output_id` as defined in your dataflow.
-    /// - the second argument is the data as either bytes or pyarrow.UInt8Array for zero copy.
-    /// - the third argument is dora metadata if you want ot link the tracing from one input into an output.
-    /// `e.g.:  send_output("bbox", pa.array([100], type=pa.uint8()), dora_event["metadata"])`
     #[pymethods]
     impl SendOutputCallback {
         fn __call__(
             &mut self,
             output: &str,
             data: PyObject,
             metadata: Option<&PyDict>,
```

### Comparing `dora_rs-0.2.4/local_dependencies/dora-runtime/src/operator/shared_lib.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-runtime/src/operator/shared_lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-tracing/Cargo.toml` & `dora_rs-0.2.4rc3/local_dependencies/dora-tracing/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-tracing"
-version= "0.2.4"
+version= "0.2.4-rc3"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `dora_rs-0.2.4/local_dependencies/dora-tracing/src/lib.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-tracing/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-tracing/src/telemetry.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-tracing/src/telemetry.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/shared-memory-server/Cargo.toml` & `dora_rs-0.2.4rc3/local_dependencies/shared-memory-server/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [package]
 name = "shared-memory-server"
-version= "0.2.4"
+version= "0.2.4-rc3"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 eyre = "0.6.8"
 serde = { version = "1.0.152", features = ["derive"] }
-shared_memory_extended = "0.13.0"
+shared_memory = "0.12.0"
 # TODO use upstream release once https://github.com/elast0ny/raw_sync-rs/pull/29 is merged
 # Current fix, use personally pushed `raw_sync_2` version.
 raw_sync_2 = "0.1.5"
 bincode = "1.3.3"
 tracing = "0.1.37"
```

### Comparing `dora_rs-0.2.4/local_dependencies/shared-memory-server/src/bin/bench.rs` & `dora_rs-0.2.4rc3/local_dependencies/shared-memory-server/src/bin/bench.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/shared-memory-server/src/channel.rs` & `dora_rs-0.2.4rc3/local_dependencies/shared-memory-server/src/channel.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use eyre::{eyre, Context};
 use raw_sync_2::events::{Event, EventImpl, EventInit, EventState};
 use serde::{Deserialize, Serialize};
-use shared_memory_extended::Shmem;
+use shared_memory::Shmem;
 use std::{
     mem, slice,
     sync::atomic::{AtomicBool, AtomicU64},
     time::Duration,
 };
 
 pub struct ShmemChannel {
```

### Comparing `dora_rs-0.2.4/local_dependencies/shared-memory-server/src/lib.rs` & `dora_rs-0.2.4rc3/local_dependencies/shared-memory-server/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use self::channel::ShmemChannel;
 use eyre::{eyre, Context};
 use serde::{Deserialize, Serialize};
-pub use shared_memory_extended::{Shmem, ShmemConf};
+pub use shared_memory::{Shmem, ShmemConf};
 use std::marker::PhantomData;
 use std::time::Duration;
 
 mod channel;
 
 pub struct ShmemServer<T, U> {
     channel: ShmemChannel,
```

### Comparing `dora_rs-0.2.4/local_dependencies/dora-message/Cargo.toml` & `dora_rs-0.2.4rc3/local_dependencies/dora-message/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-message"
-version= "0.2.4"
+version= "0.2.4-rc3"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # Building capnp schema script is disabled by default as it requires to install capnp.
 # To change the schema install capnp at: https://capnproto.org/install.html
```

### Comparing `dora_rs-0.2.4/local_dependencies/dora-message/src/lib.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-message/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-message/src/message_capnp.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-message/src/message_capnp.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-core/Cargo.toml` & `dora_rs-0.2.4rc3/local_dependencies/dora-core/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-core"
-version= "0.2.4"
+version= "0.2.4-rc3"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `dora_rs-0.2.4/local_dependencies/dora-core/src/config.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-core/src/config.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-core/src/coordinator_messages.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-core/src/coordinator_messages.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-core/src/daemon_messages.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-core/src/daemon_messages.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-core/src/descriptor/mod.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-core/src/descriptor/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-core/src/descriptor/validate.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-core/src/descriptor/validate.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-core/src/descriptor/visualize.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-core/src/descriptor/visualize.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-core/src/lib.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-core/src/topics.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-core/src/topics.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-operator-api-types/src/lib.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-operator-api-types/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-operator-api-python/Cargo.toml` & `dora_rs-0.2.4rc3/local_dependencies/dora-operator-api-python/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-operator-api-python"
-version= "0.2.4"
+version= "0.2.4-rc3"
 edition = "2021"
 
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `dora_rs-0.2.4/local_dependencies/dora-operator-api-python/src/lib.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-operator-api-python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/local_dependencies/dora-download/Cargo.toml` & `dora_rs-0.2.4rc3/local_dependencies/dora-download/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-download"
-version= "0.2.4"
+version= "0.2.4-rc3"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `dora_rs-0.2.4/local_dependencies/dora-download/src/lib.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-download/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/Cargo.toml` & `dora_rs-0.2.4rc3/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [package]
-version= "0.2.4"
+version= "0.2.4-rc3"
 name = "dora-node-api-python"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `dora_rs-0.2.4/dora/__init__.py` & `dora_rs-0.2.4rc3/dora/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from enum import Enum
 
 from .dora import *
 
 __author__ = "Dora-rs Authors"
-__version__ = "0.2.4"
+__version__ = "0.2.4-rc3"
 
 
 class DoraStatus(Enum):
     """Dora status to indicate if operator `on_input` loop
      should be stopped.
 
     Args:
```

### Comparing `dora_rs-0.2.4/src/lib.rs` & `dora_rs-0.2.4rc3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.4/Cargo.lock` & `dora_rs-0.2.4rc3/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -591,28 +591,28 @@
  "unicode-width",
  "walkdir",
  "wild",
 ]
 
 [[package]]
 name = "benchmark-example-node"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-node-api",
  "eyre",
  "futures",
  "rand",
  "tokio",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "benchmark-example-sink"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-node-api",
  "eyre",
  "tracing",
  "tracing-subscriber",
 ]
 
@@ -903,23 +903,23 @@
 dependencies = [
  "bytes",
  "memchr",
 ]
 
 [[package]]
 name = "communication-layer-pub-sub"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "flume",
  "zenoh",
 ]
 
 [[package]]
 name = "communication-layer-request-reply"
-version = "0.2.4"
+version = "0.2.4-rc3"
 
 [[package]]
 name = "concurrent-queue"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62ec6771ecfa0762d24683ee5a32ad78487a3d3afdc0fb8cae19d2c5deb50b7c"
 dependencies = [
@@ -1264,15 +1264,15 @@
  "option-ext",
  "redox_users",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "dora-cli"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "bat",
  "clap 4.3.0",
  "communication-layer-request-reply",
  "ctrlc",
  "dora-core",
  "dora-node-api-c",
@@ -1288,15 +1288,15 @@
  "tracing",
  "uuid",
  "webbrowser",
 ]
 
 [[package]]
 name = "dora-coordinator"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "clap 3.2.25",
  "ctrlc",
  "dora-core",
  "dora-tracing",
  "eyre",
  "futures",
@@ -1313,15 +1313,15 @@
  "uuid",
  "which",
  "zenoh",
 ]
 
 [[package]]
 name = "dora-core"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-message",
  "eyre",
  "once_cell",
  "serde",
  "serde-with-expand-env",
  "serde_yaml 0.9.21",
@@ -1329,15 +1329,15 @@
  "tracing",
  "uuid",
  "which",
 ]
 
 [[package]]
 name = "dora-daemon"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "async-trait",
  "bincode",
  "clap 3.2.25",
  "ctrlc",
  "dora-core",
  "dora-download",
@@ -1356,15 +1356,15 @@
  "tracing",
  "tracing-opentelemetry",
  "uuid",
 ]
 
 [[package]]
 name = "dora-download"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "eyre",
  "reqwest",
  "tokio",
  "tracing",
 ]
 
@@ -1385,148 +1385,147 @@
  "tracing",
  "tracing-subscriber",
  "uuid",
 ]
 
 [[package]]
 name = "dora-message"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "capnp",
  "capnpc",
  "serde",
  "uhlc",
 ]
 
 [[package]]
 name = "dora-metrics"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "futures",
  "opentelemetry 0.17.0",
  "opentelemetry-otlp",
  "opentelemetry-system-metrics",
  "tokio",
 ]
 
 [[package]]
 name = "dora-node-api"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "arrow",
  "bincode",
  "capnp",
  "dora-core",
  "dora-tracing",
  "eyre",
  "flume",
  "futures",
- "futures-concurrency",
  "once_cell",
  "serde",
  "serde_json",
  "serde_yaml 0.8.26",
  "shared-memory-server",
- "shared_memory_extended",
+ "shared_memory",
  "thiserror",
  "tokio",
  "tracing",
  "uuid",
 ]
 
 [[package]]
 name = "dora-node-api-c"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-node-api",
  "eyre",
  "flume",
  "tracing",
 ]
 
 [[package]]
 name = "dora-node-api-cxx"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "cxx",
  "cxx-build",
  "dora-node-api",
  "eyre",
 ]
 
 [[package]]
 name = "dora-node-api-python"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "arrow",
  "dora-node-api",
  "dora-operator-api-python",
  "dora-runtime",
  "eyre",
  "flume",
  "pyo3",
  "pythonize",
  "serde_yaml 0.8.26",
 ]
 
 [[package]]
 name = "dora-operator-api"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-operator-api-macros",
  "dora-operator-api-types",
 ]
 
 [[package]]
 name = "dora-operator-api-c"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-operator-api-types",
 ]
 
 [[package]]
 name = "dora-operator-api-cxx"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "cxx",
  "cxx-build",
  "dora-operator-api",
 ]
 
 [[package]]
 name = "dora-operator-api-macros"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "dora-operator-api-python"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "arrow",
  "dora-node-api",
  "eyre",
  "flume",
  "pyo3",
  "serde_yaml 0.8.26",
 ]
 
 [[package]]
 name = "dora-operator-api-types"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "safer-ffi",
 ]
 
 [[package]]
 name = "dora-runtime"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "clap 4.3.0",
  "dora-core",
  "dora-download",
  "dora-metrics",
  "dora-node-api",
  "dora-operator-api-python",
@@ -1547,15 +1546,15 @@
  "tracing",
  "tracing-opentelemetry",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "dora-tracing"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "eyre",
  "opentelemetry 0.18.0",
  "opentelemetry-jaeger",
  "tokio",
  "tracing",
  "tracing-opentelemetry",
@@ -1851,17 +1850,17 @@
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-concurrency"
-version = "7.3.0"
+version = "7.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b726119e6cd29cf120724495b2085e1ed3d17821ea17b86de54576d1aa565f5e"
+checksum = "30ce9739c5655304eced9aaea4220e4393b8f60a3a5f1b84d09a206d6a5078a9"
 dependencies = [
  "bitvec",
  "futures-core",
  "pin-project",
 ]
 
 [[package]]
@@ -2786,33 +2785,33 @@
 name = "multimap"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5ce46fe64a9d73be07dcbe690a38ce1b293be448fd8ce1e6c1b8062c9f72c6a"
 
 [[package]]
 name = "multiple-daemons-example-node"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-node-api",
  "eyre",
  "futures",
  "rand",
  "tokio",
 ]
 
 [[package]]
 name = "multiple-daemons-example-operator"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-operator-api",
 ]
 
 [[package]]
 name = "multiple-daemons-example-sink"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-node-api",
  "eyre",
 ]
 
 [[package]]
 name = "names"
@@ -4001,33 +4000,33 @@
  "smallvec",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "rust-dataflow-example-node"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-node-api",
  "eyre",
  "futures",
  "rand",
  "tokio",
 ]
 
 [[package]]
 name = "rust-dataflow-example-operator"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-operator-api",
 ]
 
 [[package]]
 name = "rust-dataflow-example-sink"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-node-api",
  "eyre",
 ]
 
 [[package]]
 name = "rustc-hash"
@@ -4330,33 +4329,33 @@
 checksum = "900fba806f70c630b0a382d0d825e17a0f19fcd059a2ade1ff237bcddf446b31"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "shared-memory-server"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "bincode",
  "eyre",
  "raw_sync_2",
  "serde",
- "shared_memory_extended",
+ "shared_memory",
  "tracing",
 ]
 
 [[package]]
-name = "shared_memory_extended"
-version = "0.13.0"
+name = "shared_memory"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "004d7ece9a3be64f85471d50967710b0a146144225bed5f0abd0514a3bed086f"
+checksum = "ba8593196da75d9dc4f69349682bd4c2099f8cde114257d1ef7ef1b33d1aba54"
 dependencies = [
  "cfg-if",
  "libc",
- "nix 0.26.2",
+ "nix 0.23.2",
  "rand",
  "win-sys",
 ]
 
 [[package]]
 name = "shell-escape"
 version = "0.1.5"
@@ -5883,15 +5882,15 @@
  "zenoh-link-commons",
  "zenoh-protocol-core",
  "zenoh-sync",
 ]
 
 [[package]]
 name = "zenoh-logger"
-version = "0.2.4"
+version = "0.2.4-rc3"
 dependencies = [
  "zenoh",
 ]
 
 [[package]]
 name = "zenoh-macros"
 version = "0.7.0-rc"
```

