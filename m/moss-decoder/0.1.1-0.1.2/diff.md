# Comparing `tmp/moss_decoder-0.1.1.tar.gz` & `tmp/moss_decoder-0.1.2.tar.gz`

## Comparing `moss_decoder-0.1.1.tar` & `moss_decoder-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 moss_decoder-0.1.1/Cargo.toml
--rw-r--r--   0        0        0     2835 2023-07-21 12:06:59.000000 moss_decoder-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      757 2023-07-21 07:38:32.000000 moss_decoder-0.1.1/.gitignore
--rw-r--r--   0        0        0      243 2023-07-21 07:45:09.000000 moss_decoder-0.1.1/README.md
--rw-r--r--   0        0        0  9582576 2023-07-21 12:28:16.000000 moss_decoder-0.1.1/moss_noise.raw
--rw-r--r--   0        0        0      388 2023-07-21 06:30:24.000000 moss_decoder-0.1.1/pyproject.toml
--rw-r--r--   0        0        0  4458776 2023-04-08 05:33:25.000000 moss_decoder-0.1.1/python310.dll
--rw-r--r--   0        0        0     9275 2023-07-21 12:51:01.000000 moss_decoder-0.1.1/src/lib.rs
--rw-r--r--   0        0        0     3685 2023-07-21 11:50:49.000000 moss_decoder-0.1.1/src/moss_protocol.rs
--rw-r--r--   0        0        0     7427 2023-07-21 12:52:56.000000 moss_decoder-0.1.1/Cargo.lock
--rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 moss_decoder-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 moss_decoder-0.1.2/Cargo.toml
+-rw-r--r--   0        0        0     2835 2023-07-21 12:06:59.000000 moss_decoder-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      757 2023-07-21 07:38:32.000000 moss_decoder-0.1.2/.gitignore
+-rw-r--r--   0        0        0      243 2023-07-21 07:45:09.000000 moss_decoder-0.1.2/README.md
+-rw-r--r--   0        0        0  9582576 2023-07-21 12:28:16.000000 moss_decoder-0.1.2/moss_noise.raw
+-rw-r--r--   0        0        0      388 2023-07-21 06:30:24.000000 moss_decoder-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0  4458776 2023-04-08 05:33:25.000000 moss_decoder-0.1.2/python310.dll
+-rw-r--r--   0        0        0    13621 2023-07-21 13:51:04.000000 moss_decoder-0.1.2/src/lib.rs
+-rw-r--r--   0        0        0     3685 2023-07-21 11:50:49.000000 moss_decoder-0.1.2/src/moss_protocol.rs
+-rw-r--r--   0        0        0     7427 2023-07-21 13:52:28.000000 moss_decoder-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 moss_decoder-0.1.2/PKG-INFO
```

### Comparing `moss_decoder-0.1.1/Cargo.toml` & `moss_decoder-0.1.2/Cargo.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 [package]
 name = "moss_decoder"
-version = "0.1.1"
+version = "0.1.2"
 edition = "2021"
 authors = ["Marc Beck König <mbkj@tutamail.com>"]
 license = "MIT OR Apache-2.0"
 description = "Python module providing a decoder for the MOSS chip protocol."
 categories = ["python-module"]
 
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "moss_decoder"
 crate-type = ["cdylib", "rlib"]
 
 [dependencies]
-pyo3 = { version = "0.19.1", features = ["extension-module"] }
+pyo3 = { version = "0.19.1", features = ["extension-module"] }
+
+
+[profile.release]
+codegen-units = 1
+debug = false
+incremental = false
+lto = true
+opt-level = 3
+panic = "abort"
```

### Comparing `moss_decoder-0.1.1/.github/workflows/CI.yml` & `moss_decoder-0.1.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.1.1/.gitignore` & `moss_decoder-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.1.1/moss_noise.raw` & `moss_decoder-0.1.2/moss_noise.raw`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.1.1/python310.dll` & `moss_decoder-0.1.2/python310.dll`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.1.1/src/lib.rs` & `moss_decoder-0.1.2/src/lib.rs`

 * *Files 23% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 use moss_protocol::MossWord;
 
 /// A Python module for decoding raw MOSS data in Rust.
 #[pymodule]
 fn moss_decoder(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(decode_event, m)?)?;
     m.add_function(wrap_pyfunction!(decode_multiple_events, m)?)?;
+    m.add_function(wrap_pyfunction!(decode_multiple_events_alt, m)?)?;
 
     m.add_class::<MossHit>()?;
     m.add_class::<MossPacket>()?;
 
     Ok(())
 }
 
@@ -98,14 +99,105 @@
     if moss_packets.is_empty() {
         Err(PyTypeError::new_err("No MOSS Packets in events"))
     } else {
         Ok(moss_packets)
     }
 }
 
+/// Decodes multiple MOSS events into a list of [MossPacket]s
+#[pyfunction]
+fn decode_multiple_events_alt(bytes: &[u8]) -> PyResult<(Vec<MossPacket>, usize)> {
+    let byte_cnt = bytes.len();
+
+    if byte_cnt < 6 {
+        return Err(PyTypeError::new_err(
+            "Received less than the minimum event size",
+        ));
+    }
+
+    let mut moss_packets: Vec<MossPacket> = Vec::with_capacity(byte_cnt / 1024);
+
+    let mut last_trailer_idx = 0;
+
+    let mut is_moss_packet = false;
+    //let mut current_unit_id = 0xff; // placeholder
+    let mut current_region: u8 = 0xff; // placeholder
+
+    for (i, byte) in bytes.iter().enumerate() {
+        if let Ok(word) = MossWord::from_byte(*byte) {
+            match word {
+                MossWord::Idle => (),
+                MossWord::UnitFrameHeader => {
+                    debug_assert!(!is_moss_packet);
+                    is_moss_packet = true;
+                    moss_packets.push(MossPacket {
+                        unit_id: *byte & 0x0F,
+                        hits: Vec::new(),
+                    });
+                }
+                MossWord::UnitFrameTrailer => {
+                    debug_assert!(is_moss_packet);
+                    is_moss_packet = false;
+                    last_trailer_idx = i;
+                }
+                MossWord::RegionHeader => {
+                    debug_assert!(is_moss_packet);
+                    current_region = *byte & 0x03;
+                }
+                MossWord::Data0 => {
+                    debug_assert!(is_moss_packet);
+                    moss_packets.last_mut().unwrap().hits.push(MossHit {
+                        region: current_region,            // region id
+                        row: ((*byte & 0x3F) as u16) << 3, // row position [8:3]
+                        column: 0,                         // placeholder
+                    });
+                }
+                MossWord::Data1 => {
+                    debug_assert!(is_moss_packet);
+                    // row position [2:0]
+                    moss_packets
+                        .last_mut()
+                        .unwrap()
+                        .hits
+                        .last_mut()
+                        .unwrap()
+                        .row |= ((*byte & 0x38) >> 3) as u16;
+                    // col position [8:6]
+                    moss_packets
+                        .last_mut()
+                        .unwrap()
+                        .hits
+                        .last_mut()
+                        .unwrap()
+                        .column = ((*byte & 0x07) as u16) << 6;
+                }
+                MossWord::Data2 => {
+                    debug_assert!(is_moss_packet);
+                    moss_packets
+                        .last_mut()
+                        .unwrap()
+                        .hits
+                        .last_mut()
+                        .unwrap()
+                        .column |= (*byte & 0x3F) as u16; // col position [5:0]
+                }
+                MossWord::Delimiter => {
+                    debug_assert!(!is_moss_packet);
+                }
+            }
+        }
+    }
+
+    if moss_packets.is_empty() {
+        Err(PyTypeError::new_err("No MOSS Packets in events"))
+    } else {
+        Ok((moss_packets, last_trailer_idx))
+    }
+}
+
 #[cfg(test)]
 mod tests {
     use super::*;
 
     const IDLE: u8 = 0xFF;
     const UNIT_FRAME_TRAILER: u8 = 0xE0;
     const UNIT_FRAME_HEADER_0: u8 = 0xD0;
@@ -284,14 +376,30 @@
 
         for p in moss_packets {
             println!("{p:?}");
         }
     }
 
     #[test]
+    fn test_decoding_multiple_events_alt() {
+        let events = fake_multiple_events();
+
+        let (packets, unprocessed_data) = decode_multiple_events_alt(&events).unwrap();
+
+        let packet_count = packets.len();
+
+        println!("last trailer at idx: {unprocessed_data}");
+        println!("{packet_count}");
+
+        for p in packets {
+            println!("{p:?}");
+        }
+    }
+
+    #[test]
     fn test_decoding_multiple_events_delimiter() {
         let mut events = fake_multiple_events();
         events.append(&mut vec![0xFA, 0xFA, 0xFA]);
 
         let mut moss_packets: Vec<MossPacket> = Vec::new();
 
         while let Ok((packet, unprocessed_data)) = decode_event(events) {
@@ -305,15 +413,27 @@
 
         for p in moss_packets {
             println!("{p:?}");
         }
     }
 
     #[test]
+    #[ignore = "local test file needed"]
     fn test_read_file_decode() {
+        let time = std::time::Instant::now();
+
+        println!("Reading file...");
         let f = std::fs::read(std::path::PathBuf::from("../moss_noise.raw")).unwrap();
+        println!(
+            "Read file in: {t:?}. Bytes: {cnt}",
+            t = time.elapsed(),
+            cnt = f.len()
+        );
 
-        let p = decode_multiple_events(f).unwrap();
+        println!("Decoding content...");
+        let (p, last_trailer_idx) = decode_multiple_events_alt(&f).unwrap();
+        println!("Decoded in: {t:?}\n", t = time.elapsed());
 
         println!("Got: {packets}", packets = p.len());
+        println!("Last trailer at index: {last_trailer_idx}");
     }
 }
```

### Comparing `moss_decoder-0.1.1/src/moss_protocol.rs` & `moss_decoder-0.1.2/src/moss_protocol.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.1.1/Cargo.lock` & `moss_decoder-0.1.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "moss_decoder"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.18.0"
```

### Comparing `moss_decoder-0.1.1/PKG-INFO` & `moss_decoder-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moss_decoder
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Python module providing a decoder for the MOSS chip protocol.
 Author: Marc Beck König <mbkj@tutamail.com>
 Author-email: Marc Beck König <mbkj@tutamail.com>
 License: MIT OR Apache-2.0
```

