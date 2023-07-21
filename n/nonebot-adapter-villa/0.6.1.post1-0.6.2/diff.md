# Comparing `tmp/nonebot_adapter_villa-0.6.1.post1.tar.gz` & `tmp/nonebot_adapter_villa-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_villa-0.6.1.post1.tar", max compression
+gzip compressed data, was "nonebot_adapter_villa-0.6.2.tar", max compression
```

## Comparing `nonebot_adapter_villa-0.6.1.post1.tar` & `nonebot_adapter_villa-0.6.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1062 2023-07-18 12:46:44.014352 nonebot_adapter_villa-0.6.1.post1/LICENSE
--rw-r--r--   0        0        0     7323 2023-07-18 12:46:44.014352 nonebot_adapter_villa-0.6.1.post1/README.md
--rw-r--r--   0        0        0      228 2023-07-18 12:46:44.014352 nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/__init__.py
--rw-r--r--   0        0        0    12154 2023-07-18 12:46:44.014352 nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/adapter.py
--rw-r--r--   0        0        0      114 2023-07-18 12:46:44.014352 nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/api/__init__.py
--rw-r--r--   0        0        0       25 2023-07-18 12:46:44.014352 nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/api/client.py
--rw-r--r--   0        0        0     3293 2023-07-18 12:46:44.014352 nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/api/client.pyi
--rw-r--r--   0        0        0    13152 2023-07-18 12:46:44.014352 nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/api/handle.py
--rw-r--r--   0        0        0     9488 2023-07-18 12:46:44.014352 nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/api/models.py
--rw-r--r--   0        0        0     1734 2023-07-18 12:46:44.014352 nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/api/request.py
--rw-r--r--   0        0        0    14467 2023-07-18 12:46:44.014352 nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/bot.py
--rw-r--r--   0        0        0     1190 2023-07-18 12:46:44.014352 nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/config.py
--rw-r--r--   0        0        0    12798 2023-07-18 12:46:44.014352 nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/event.py
--rw-r--r--   0        0        0     2717 2023-07-18 12:46:44.018352 nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/exception.py
--rw-r--r--   0        0        0     9952 2023-07-18 12:46:44.018352 nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/message.py
--rw-r--r--   0        0        0     1449 2023-07-18 12:46:44.018352 nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/permission.py
--rw-r--r--   0        0        0       76 2023-07-18 12:46:44.018352 nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/utils.py
--rw-r--r--   0        0        0     2130 2023-07-18 12:46:44.018352 nonebot_adapter_villa-0.6.1.post1/pyproject.toml
--rw-r--r--   0        0        0     8255 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.6.1.post1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-21 07:37:21.910586 nonebot_adapter_villa-0.6.2/LICENSE
+-rw-r--r--   0        0        0     7323 2023-07-21 07:37:21.910586 nonebot_adapter_villa-0.6.2/README.md
+-rw-r--r--   0        0        0      228 2023-07-21 07:37:21.910586 nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/__init__.py
+-rw-r--r--   0        0        0    12154 2023-07-21 07:37:21.910586 nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/adapter.py
+-rw-r--r--   0        0        0      114 2023-07-21 07:37:21.910586 nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/api/__init__.py
+-rw-r--r--   0        0        0       25 2023-07-21 07:37:21.910586 nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/api/client.py
+-rw-r--r--   0        0        0     3293 2023-07-21 07:37:21.914586 nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/api/client.pyi
+-rw-r--r--   0        0        0    13152 2023-07-21 07:37:21.914586 nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/api/handle.py
+-rw-r--r--   0        0        0     9534 2023-07-21 07:37:21.914586 nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/api/models.py
+-rw-r--r--   0        0        0     1734 2023-07-21 07:37:21.914586 nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/api/request.py
+-rw-r--r--   0        0        0    14467 2023-07-21 07:37:21.914586 nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/bot.py
+-rw-r--r--   0        0        0     1190 2023-07-21 07:37:21.914586 nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/config.py
+-rw-r--r--   0        0        0    12798 2023-07-21 07:37:21.914586 nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/event.py
+-rw-r--r--   0        0        0     2717 2023-07-21 07:37:21.914586 nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/exception.py
+-rw-r--r--   0        0        0     9952 2023-07-21 07:37:21.914586 nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/message.py
+-rw-r--r--   0        0        0     1449 2023-07-21 07:37:21.914586 nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/permission.py
+-rw-r--r--   0        0        0       76 2023-07-21 07:37:21.914586 nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/utils.py
+-rw-r--r--   0        0        0     2125 2023-07-21 07:37:21.914586 nonebot_adapter_villa-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     8249 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.6.2/PKG-INFO
```

### Comparing `nonebot_adapter_villa-0.6.1.post1/LICENSE` & `nonebot_adapter_villa-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.1.post1/README.md` & `nonebot_adapter_villa-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/adapter.py` & `nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/api/client.pyi` & `nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/api/client.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/api/handle.py` & `nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/api/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/api/models.py` & `nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/api/models.py`

 * *Files 1% similar despite different names*

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

### Comparing `nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/api/request.py` & `nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/bot.py` & `nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/config.py` & `nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/event.py` & `nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/exception.py` & `nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/message.py` & `nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.1.post1/nonebot/adapters/villa/permission.py` & `nonebot_adapter_villa-0.6.2/nonebot/adapters/villa/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.1.post1/pyproject.toml` & `nonebot_adapter_villa-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-villa"
-version = "0.6.1post1"
+version = "0.6.2"
 description = "NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 repository = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 documentation = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
```

### Comparing `nonebot_adapter_villa-0.6.1.post1/PKG-INFO` & `nonebot_adapter_villa-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-villa
-Version: 0.6.1.post1
+Version: 0.6.2
 Summary: NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa
 License: MIT
 Keywords: nonebot,mihoyo,bot
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.6.1.post1 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.6.2 Summary:
 NoneBot2ç±³æ¸¸ç¤¾å¤§å«éBotééå¨ãMiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa License: MIT
 Keywords: nonebot,mihoyo,bot Author: CMHopeSunshine Author-email:
 277073121@qq.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

