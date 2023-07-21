# Comparing `tmp/aioconnection-0.1.2-py3-none-win_amd64.whl.zip` & `tmp/aioconnection-0.1.3-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 11212 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      280 b- defN 23-Mar-03 09:24 aioconnection/__init__.py
--rw-rw-rw-  2.0 fat    10710 b- defN 23-Mar-03 09:24 aioconnection/protocol.py
--rw-rw-rw-  2.0 fat      401 b- defN 23-Mar-03 09:24 aioconnection/utils.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-03 09:24 aioconnection/transport/__init__.py
--rw-rw-rw-  2.0 fat      152 b- defN 23-Mar-03 09:24 aioconnection/transport/serialport/__init__.py
--rw-rw-rw-  2.0 fat    10014 b- defN 23-Mar-03 09:24 aioconnection/transport/serialport/core.py
--rw-rw-rw-  2.0 fat     5934 b- defN 23-Mar-03 09:24 aioconnection/transport/serialport/transport.py
--rw-rw-rw-  2.0 fat     1096 b- defN 23-Mar-03 09:24 aioconnection-0.1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      823 b- defN 23-Mar-03 09:24 aioconnection-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       98 b- defN 23-Mar-03 09:24 aioconnection-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Mar-03 09:24 aioconnection-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1052 b- defN 23-Mar-03 09:24 aioconnection-0.1.2.dist-info/RECORD
-12 files, 30574 bytes uncompressed, 9416 bytes compressed:  69.2%
+Zip file size: 11252 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      280 b- defN 23-Jul-21 07:51 aioconnection/__init__.py
+-rw-rw-rw-  2.0 fat    10906 b- defN 23-Jul-21 07:51 aioconnection/protocol.py
+-rw-rw-rw-  2.0 fat      401 b- defN 23-Jul-21 07:51 aioconnection/utils.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-21 07:51 aioconnection/transport/__init__.py
+-rw-rw-rw-  2.0 fat      152 b- defN 23-Jul-21 07:51 aioconnection/transport/serialport/__init__.py
+-rw-rw-rw-  2.0 fat    10014 b- defN 23-Jul-21 07:51 aioconnection/transport/serialport/core.py
+-rw-rw-rw-  2.0 fat     5934 b- defN 23-Jul-21 07:51 aioconnection/transport/serialport/transport.py
+-rw-rw-rw-  2.0 fat     1096 b- defN 23-Jul-21 07:52 aioconnection-0.1.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      823 b- defN 23-Jul-21 07:52 aioconnection-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       98 b- defN 23-Jul-21 07:52 aioconnection-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jul-21 07:52 aioconnection-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1052 b- defN 23-Jul-21 07:52 aioconnection-0.1.3.dist-info/RECORD
+12 files, 30770 bytes uncompressed, 9456 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: aioconnection/transport/serialport/core.py
 Comment: 
 
 Filename: aioconnection/transport/serialport/transport.py
 Comment: 
 
-Filename: aioconnection-0.1.2.dist-info/LICENSE
+Filename: aioconnection-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: aioconnection-0.1.2.dist-info/METADATA
+Filename: aioconnection-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: aioconnection-0.1.2.dist-info/WHEEL
+Filename: aioconnection-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: aioconnection-0.1.2.dist-info/top_level.txt
+Filename: aioconnection-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: aioconnection-0.1.2.dist-info/RECORD
+Filename: aioconnection-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aioconnection/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
 from .protocol import (
     Protocol,
     TAIL_SENTINEL,
     Parser,
     StrParser,
     RawParser,
```

## aioconnection/protocol.py

```diff
@@ -165,15 +165,15 @@
         self.transport_info: t.Optional[TransportInfo] = None
         self.reply_timeout = reply_timeout
         # TODO write id to class
         self._write_id = 0
         self._next_write_id = 0
         self._loop: asyncio.AbstractEventLoop = loop or asyncio.get_event_loop()
         self._in_buffer: bytes = b''
-        self._out_buffer: deque[tuple[list[bytes, t.Any], float]] = deque()
+        self._out_buffer: deque[tuple[list, float]] = deque()
         self._allowed_to_write = False
         self._reply_awaiting = False
         # TODO maybe create cancelled task and handle
         self._reply_handle: t.Optional[asyncio.Handle] = None
         self._recv_last_time = 0.0
         self._idle_timeout = idle_timeout
         self._ping_task: t.Optional[asyncio.Task] = None
@@ -221,28 +221,31 @@
         self._reply_expired(False)
         self.transport_info = TransportInfo.make(self.transport, exc)
         self._register_event(Etype.CONNECT_FAILED, data=self.transport_info)
 
     def connection_lost(self, exc):
         self.connection_failed(exc)
 
-    def data_received(self, data_raw):
-        self._recv_last_time = ftime()
-        time_ = self.event_ftime()
-        event_type = Etype.RECV
-        data_raw = self._in_buffer + data_raw if self._in_buffer else data_raw
-        bytes_data = list(self.parser.process(data_raw))
-        self._in_buffer = b''
-        is_reply = bool(self._reply_handle)
-        for bytes_, data in bytes_data:
-            if data is TAIL_SENTINEL:
-                self._in_buffer = bytes_
-                continue
-            self._register_event(event_type, bytes_, data, time_,
-                                 set_id=is_reply, set_reply=is_reply)
+    def data_received(self, data_raw: bytes, force: bool = False):
+        if self._allowed_to_write or force:
+            self._recv_last_time = ftime()
+            time_ = self.event_ftime()
+            event_type = Etype.RECV
+            data_raw = self._in_buffer + data_raw if self._in_buffer else data_raw
+            bytes_data = list(self.parser.process(data_raw))
+            self._in_buffer = b''
+            is_reply = bool(self._reply_handle)
+            for bytes_, data in bytes_data:
+                if data is TAIL_SENTINEL:
+                    self._in_buffer = bytes_
+                    continue
+                self._register_event(event_type, bytes_, data, time_,
+                                     set_id=is_reply, set_reply=is_reply)
+        else:
+            self._loop.call_soon(self.data_received, data_raw, True)
 
     def _reply_expired(self, accepted=True):
         if self._reply_handle:
             self._reply_handle.cancel()
             self._reply_handle = None
             if not accepted:
                 self._register_event(Etype.REPLY_EXPIRED, set_id=True)
```

## Comparing `aioconnection-0.1.2.dist-info/LICENSE` & `aioconnection-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aioconnection-0.1.2.dist-info/METADATA` & `aioconnection-0.1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioconnection
-Version: 0.1.2
+Version: 0.1.3
 Summary: Async messaging
 Home-page: https://github.com/means0nothing/AioConnection
 Author: Pavel Shevcov
 Author-email: means0nothing@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

## Comparing `aioconnection-0.1.2.dist-info/RECORD` & `aioconnection-0.1.3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-aioconnection/__init__.py,sha256=EFFHxeTQrjFbAz56yVXUrpVzW8jYr58c_ER8rvZT2H0,280
-aioconnection/protocol.py,sha256=aP60RTB4TOALPflLjTU2JFzABXm7mYRijADG4DJ73oM,10710
+aioconnection/__init__.py,sha256=hbvpRRp7ItvlmmOxXEa3O2mHdcASBAnwHBqrWMhmwXY,280
+aioconnection/protocol.py,sha256=EHthqjSLBsWrjiEff558ORtIYv3H8rac964Vkn4nNJc,10906
 aioconnection/utils.py,sha256=QliBbP00mgwbQ0AbJMPmOQ8nE1rP0jYElX4GIxAoTbQ,401
 aioconnection/transport/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aioconnection/transport/serialport/__init__.py,sha256=urkjBupdKJ5JwNeNaSYWk0MQMttenb6JyPOJ2UVw8QM,152
 aioconnection/transport/serialport/core.py,sha256=e0L13VHh455WOlMsX_I6GqIezCkukjSXt5NJeydqlcY,10014
 aioconnection/transport/serialport/transport.py,sha256=42TvqNStpee4zKhZTyB_wiXAUZBFjou2YfY7NbuUNDw,5934
-aioconnection-0.1.2.dist-info/LICENSE,sha256=KOI2v5c_M5MQQkVqxM4BBqmkZnNAh6PYV-3Q9pTInWE,1096
-aioconnection-0.1.2.dist-info/METADATA,sha256=uJjhVVDOMH2tYvL484btOBuHh2oNC0DqOyf7FenyQbE,823
-aioconnection-0.1.2.dist-info/WHEEL,sha256=AiyVnrmrEuW_cPqhPlarzpb5qtD8ITcBeZKvhXXgyN4,98
-aioconnection-0.1.2.dist-info/top_level.txt,sha256=AvMLNfAMAdyTsRY--I6X5S70SLUcDAYMYbPmuFGHXSs,14
-aioconnection-0.1.2.dist-info/RECORD,,
+aioconnection-0.1.3.dist-info/LICENSE,sha256=KOI2v5c_M5MQQkVqxM4BBqmkZnNAh6PYV-3Q9pTInWE,1096
+aioconnection-0.1.3.dist-info/METADATA,sha256=ovNIDR5kf_yRMR1tEcm7_m384QmJnpDpUhfffpG_Pso,823
+aioconnection-0.1.3.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+aioconnection-0.1.3.dist-info/top_level.txt,sha256=AvMLNfAMAdyTsRY--I6X5S70SLUcDAYMYbPmuFGHXSs,14
+aioconnection-0.1.3.dist-info/RECORD,,
```

