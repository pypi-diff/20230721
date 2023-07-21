# Comparing `tmp/villa-0.7.1.tar.gz` & `tmp/villa-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "villa-0.7.1.tar", max compression
+gzip compressed data, was "villa-0.7.2.tar", max compression
```

## Comparing `villa-0.7.1.tar` & `villa-0.7.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1062 2023-07-17 10:49:59.663911 villa-0.7.1/LICENSE
--rw-r--r--   0        0        0     3747 2023-07-17 10:49:59.663911 villa-0.7.1/README.md
--rw-r--r--   0        0        0     2140 2023-07-17 10:49:59.663911 villa-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      277 2023-07-17 10:49:59.663911 villa-0.7.1/villa/__init__.py
--rw-r--r--   0        0        0    40693 2023-07-17 10:49:59.663911 villa-0.7.1/villa/bot.py
--rw-r--r--   0        0        0    12215 2023-07-17 10:49:59.663911 villa-0.7.1/villa/event.py
--rw-r--r--   0        0        0     1835 2023-07-17 10:49:59.663911 villa-0.7.1/villa/exception.py
--rw-r--r--   0        0        0     3337 2023-07-17 10:49:59.663911 villa-0.7.1/villa/handle.py
--rw-r--r--   0        0        0     1537 2023-07-17 10:49:59.663911 villa-0.7.1/villa/log.py
--rw-r--r--   0        0        0    21359 2023-07-17 10:49:59.663911 villa-0.7.1/villa/message.py
--rw-r--r--   0        0        0     9304 2023-07-17 10:49:59.663911 villa-0.7.1/villa/models.py
--rw-r--r--   0        0        0      935 2023-07-17 10:49:59.663911 villa-0.7.1/villa/store.py
--rw-r--r--   0        0        0      240 2023-07-17 10:49:59.663911 villa-0.7.1/villa/typing.py
--rw-r--r--   0        0        0      968 2023-07-17 10:49:59.663911 villa-0.7.1/villa/utils.py
--rw-r--r--   0        0        0     4731 1970-01-01 00:00:00.000000 villa-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-21 07:44:11.656905 villa-0.7.2/LICENSE
+-rw-r--r--   0        0        0     3747 2023-07-21 07:44:11.656905 villa-0.7.2/README.md
+-rw-r--r--   0        0        0     2140 2023-07-21 07:44:11.656905 villa-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      277 2023-07-21 07:44:11.656905 villa-0.7.2/villa/__init__.py
+-rw-r--r--   0        0        0    40762 2023-07-21 07:44:11.656905 villa-0.7.2/villa/bot.py
+-rw-r--r--   0        0        0    12215 2023-07-21 07:44:11.656905 villa-0.7.2/villa/event.py
+-rw-r--r--   0        0        0     1835 2023-07-21 07:44:11.656905 villa-0.7.2/villa/exception.py
+-rw-r--r--   0        0        0     3337 2023-07-21 07:44:11.656905 villa-0.7.2/villa/handle.py
+-rw-r--r--   0        0        0     1537 2023-07-21 07:44:11.656905 villa-0.7.2/villa/log.py
+-rw-r--r--   0        0        0    21359 2023-07-21 07:44:11.656905 villa-0.7.2/villa/message.py
+-rw-r--r--   0        0        0     9350 2023-07-21 07:44:11.656905 villa-0.7.2/villa/models.py
+-rw-r--r--   0        0        0      935 2023-07-21 07:44:11.656905 villa-0.7.2/villa/store.py
+-rw-r--r--   0        0        0      240 2023-07-21 07:44:11.656905 villa-0.7.2/villa/typing.py
+-rw-r--r--   0        0        0     1534 2023-07-21 07:44:11.656905 villa-0.7.2/villa/utils.py
+-rw-r--r--   0        0        0     4731 1970-01-01 00:00:00.000000 villa-0.7.2/PKG-INFO
```

### Comparing `villa-0.7.1/LICENSE` & `villa-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `villa-0.7.1/README.md` & `villa-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `villa-0.7.1/pyproject.toml` & `villa-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "villa"
-version = "0.7.1"
+version = "0.7.2"
 description = "米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/villa-py"
 repository = "https://github.com/CMHopeSunshine/villa-py"
 documentation = "https://github.com/CMHopeSunshine/villa-py"
```

### Comparing `villa-0.7.1/villa/bot.py` & `villa-0.7.2/villa/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     MessageSegment,
     RoomLink as RoomLinkSegment,
     Text as TextSegment,
 )
 from .models import *
 from .store import get_app, get_bot, store_bot
 from .typing import T_Func, T_Handler
-from .utils import escape_tag
+from .utils import escape_tag, format_pub_key
 
 from fastapi import BackgroundTasks, FastAPI, Request
 from fastapi.responses import JSONResponse
 import httpx
 from httpx._types import TimeoutTypes
 from pydantic import parse_obj_as
 import rsa
@@ -82,16 +82,17 @@
             bot_secret: 机器人密钥
             pub_key: 机器人 pub_key
             callback_url: 事件回调地址
             wait_util_complete: 是否等待事件处理完成后响应
             api_timeout: API 调用超时时间
             verify_event: 是否对事件进行验证
         """
-        if isinstance(pub_key, str):
-            pub_key = pub_key.encode()
+        if isinstance(pub_key, bytes):
+            pub_key = pub_key.decode()
+        pub_key = format_pub_key(pub_key).encode()
         self.bot_id = bot_id
         self.bot_secret = bot_secret
         self.pub_key = rsa.PublicKey.load_pkcs1_openssl_pem(pub_key)
         self.bot_secret_encrypt = hmac.new(
             pub_key,
             bot_secret.encode(),
             hashlib.sha256,
```

### Comparing `villa-0.7.1/villa/event.py` & `villa-0.7.2/villa/event.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.1/villa/exception.py` & `villa-0.7.2/villa/exception.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.1/villa/handle.py` & `villa-0.7.2/villa/handle.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.1/villa/log.py` & `villa-0.7.2/villa/log.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.1/villa/message.py` & `villa-0.7.2/villa/message.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.1/villa/models.py` & `villa-0.7.2/villa/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,14 +250,15 @@
     send_msg_auth_range: Optional["SendMsgAuthRange"] = None
 
 
 class RoomType(str, Enum):
     CHAT = "BOT_PLATFORM_ROOM_TYPE_CHAT_ROOM"
     POST = "BOT_PLATFORM_ROOM_TYPE_POST_ROOM"
     SCENE = "BOT_PLATFORM_ROOM_TYPE_SCENE_ROOM"
+    LIVE = "BOT_PLATFORM_ROOM_TYPE_LIVE_ROOM"
     INVALID = "BOT_PLATFORM_ROOM_TYPE_INVALID"
 
     def __repr__(self) -> str:
         return self.name
 
 
 class RoomDefaultNotifyType(str, Enum):
```

### Comparing `villa-0.7.1/villa/store.py` & `villa-0.7.2/villa/store.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.1/PKG-INFO` & `villa-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: villa
-Version: 0.7.1
+Version: 0.7.2
 Summary: 米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK.
 Home-page: https://github.com/CMHopeSunshine/villa-py
 License: MIT
 Keywords: mihoyo,bot,villa
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

