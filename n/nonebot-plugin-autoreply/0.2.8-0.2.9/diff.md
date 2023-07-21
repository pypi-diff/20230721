# Comparing `tmp/nonebot_plugin_autoreply-0.2.8.tar.gz` & `tmp/nonebot_plugin_autoreply-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_autoreply-0.2.8.tar", last modified: Thu Apr 27 14:44:43 2023, max compression
+gzip compressed data, was "nonebot_plugin_autoreply-0.2.9.tar", last modified: Fri Apr 28 09:29:04 2023, max compression
```

## Comparing `nonebot_plugin_autoreply-0.2.8.tar` & `nonebot_plugin_autoreply-0.2.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-04-27 14:44:33.147591 nonebot_plugin_autoreply-0.2.8/LICENSE
--rw-r--r--   0        0        0    13133 2023-04-27 14:44:33.147591 nonebot_plugin_autoreply-0.2.8/README.md
--rw-r--r--   0        0        0      303 2023-04-27 14:44:33.147591 nonebot_plugin_autoreply-0.2.8/nonebot_plugin_autoreply/__init__.py
--rw-r--r--   0        0        0     6557 2023-04-27 14:44:33.147591 nonebot_plugin_autoreply-0.2.8/nonebot_plugin_autoreply/__main__.py
--rw-r--r--   0        0        0     3623 2023-04-27 14:44:33.147591 nonebot_plugin_autoreply-0.2.8/nonebot_plugin_autoreply/config.py
--rw-r--r--   0        0        0       49 2023-04-27 14:44:33.147591 nonebot_plugin_autoreply-0.2.8/nonebot_plugin_autoreply/cool_down.py
--rw-r--r--   0        0        0     2001 2023-04-27 14:44:33.147591 nonebot_plugin_autoreply-0.2.8/nonebot_plugin_autoreply/util.py
--rw-r--r--   0        0        0      629 2023-04-27 14:44:43.583599 nonebot_plugin_autoreply-0.2.8/pyproject.toml
--rw-r--r--   0        0        0    13701 1970-01-01 00:00:00.000000 nonebot_plugin_autoreply-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-28 09:28:54.404648 nonebot_plugin_autoreply-0.2.9/LICENSE
+-rw-r--r--   0        0        0     5977 2023-04-28 09:28:54.404648 nonebot_plugin_autoreply-0.2.9/README.md
+-rw-r--r--   0        0        0      303 2023-04-28 09:28:54.404648 nonebot_plugin_autoreply-0.2.9/nonebot_plugin_autoreply/__init__.py
+-rw-r--r--   0        0        0     6803 2023-04-28 09:28:54.404648 nonebot_plugin_autoreply-0.2.9/nonebot_plugin_autoreply/__main__.py
+-rw-r--r--   0        0        0     3617 2023-04-28 09:28:54.404648 nonebot_plugin_autoreply-0.2.9/nonebot_plugin_autoreply/config.py
+-rw-r--r--   0        0        0       49 2023-04-28 09:28:54.404648 nonebot_plugin_autoreply-0.2.9/nonebot_plugin_autoreply/cool_down.py
+-rw-r--r--   0        0        0     2305 2023-04-28 09:28:54.404648 nonebot_plugin_autoreply-0.2.9/nonebot_plugin_autoreply/util.py
+-rw-r--r--   0        0        0      649 2023-04-28 09:29:04.672807 nonebot_plugin_autoreply-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     6573 1970-01-01 00:00:00.000000 nonebot_plugin_autoreply-0.2.9/PKG-INFO
```

### Comparing `nonebot_plugin_autoreply-0.2.8/LICENSE` & `nonebot_plugin_autoreply-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_autoreply-0.2.8/nonebot_plugin_autoreply/__main__.py` & `nonebot_plugin_autoreply-0.2.9/nonebot_plugin_autoreply/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -155,62 +155,63 @@
         if reply.block:
             break
 
     state["reply"] = state_reply
     return bool(state_reply)
 
 
-def get_reply_msgs(
+ReplyMessagesType = Tuple[List[Message], Optional[Tuple[int, int]]]
+
+
+async def get_reply_msgs(
     reply: ReplyType,
     var_dict: VarDictType,
     refuse_multi: bool = False,
-) -> Tuple[List[Message], Optional[Tuple[int, int]]]:
+) -> ReplyMessagesType:
     if isinstance(reply, str):
-        str_is_plain = reply.startswith("@")
-        if str_is_plain:
+        is_plain = reply.startswith("@")
+        if is_plain:
             reply = reply[1:]
 
-        reply = ReplyModel(type="plain" if str_is_plain else "normal", message=reply)
+        reply = ReplyModel(type="plain" if is_plain else "normal", message=reply)
 
     elif isinstance(reply, list):
         reply = ReplyModel(type="array", message=reply)
 
     rt = reply.type
     msg = reply.message
 
     if rt == "plain":
-        return [Message() + cast(str, msg)], None
+        msg = cast(str, msg)
+        return [Message() + msg], None
 
     if rt == "array":
-        return (
-            [
-                replace_message_var(
-                    Message(
-                        MessageSegment(type=x.type, data=x.data)
-                        for x in cast(List[MessageSegmentModel], msg)
-                    ),
-                    var_dict,
-                ),
-            ],
-            None,
-        )
+        msg = cast(List[MessageSegmentModel], msg)
+        msg = Message(MessageSegment(type=x.type, data=x.data) for x in msg)
+        msg = await replace_message_var(msg, var_dict)
+        return [msg], None
 
     if rt == "multi":
         if refuse_multi:
             raise ValueError("Nested `multi` is not allowed")
-        return (
-            [
-                get_reply_msgs(x, var_dict, True)[0][0]
-                for x in cast(List[ReplyModel], msg)
-            ],
-            reply.delay,
-        )
+
+        delay = reply.delay
+        if isinstance(delay, int):
+            delay = (delay, delay)
+
+        msg = cast(List[ReplyModel], msg)
+        msgs = [(await get_reply_msgs(x, var_dict, True))[0][0] for x in msg]
+        if reply.shuffle:
+            random.shuffle(msgs)
+
+        return msgs, delay
 
     # default normal
-    return [replace_message_var(Message(cast(str, msg)), var_dict)], None
+    msg = cast(str, msg)
+    return [await replace_message_var(Message(msg), var_dict)], None
 
 
 message_matcher = on_message(
     rule=message_checker,
     block=config.autoreply_block,
     priority=config.autoreply_priority,
 )
@@ -229,22 +230,27 @@
     event: Union[MessageEvent, PokeNotifyEvent],
     matcher: Matcher,
     state: T_State,
 ):
     reply: List[ReplyType] = state["reply"]
 
     var_dict = await get_var_dict(bot, event)
-    reply_msgs = [get_reply_msgs(x, var_dict) for x in reply]
+    reply_msgs: List[ReplyMessagesType] = await asyncio.gather(
+        *(get_reply_msgs(x, var_dict) for x in reply),
+    )
 
-    for msgs, delay in reply_msgs:
+    for msgs, delay_tuple in reply_msgs:
         for x in msgs:
             await matcher.send(x)
 
-        if delay:
-            await asyncio.sleep(random.randint(*delay) / 1000)
+        if delay_tuple:
+            d_min, d_max = delay_tuple
+            delay = d_min if d_min == d_max else random.randint(d_min, d_max)
+            delay /= 1000
+            await asyncio.sleep(delay)
 
 
 reload_matcher = on_command("重载自动回复", permission=SUPERUSER)
 
 
 @reload_matcher.handle()
 async def _(matcher: Matcher):
```

### Comparing `nonebot_plugin_autoreply-0.2.8/nonebot_plugin_autoreply/config.py` & `nonebot_plugin_autoreply-0.2.9/nonebot_plugin_autoreply/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,16 @@
     type: str  # noqa: A003
     data: Dict[str, Any]
 
 
 class ReplyModel(BaseModel):
     type: Literal["normal", "plain", "array", "multi"]  # noqa: A003
     message: MessageType
-    delay: Tuple[int, int] = (0, 0)
+    shuffle: bool = False
+    delay: Union[Tuple[int, int], int] = (0, 0)
 
 
 class FilterModel(BaseModel, Generic[T]):
     type: Literal["black", "white"] = "black"  # noqa: A003
     values: List[T]
 
 
@@ -131,15 +132,13 @@
 
         else:
             logger.opt(colors=True).info(f"加载回复配置 <y>{file_name}</y> <l><g>成功</g></l>")
             success += 1
 
     replies.sort(key=lambda x: x.priority)
     logger.opt(colors=True).info(
-        "加载回复配置完毕，"
-        f"<l><g>成功</g></l> <y>{success}</y> 个，"
-        f"<l><r>失败</r></l> <y>{fail}</y> 个",
+        f"加载回复配置完毕，<l>成功 <g>{success}</g> 个，失败 <r>{fail}</r> 个</l>",
     )
     return success, fail
 
 
 reload_replies()
```

### Comparing `nonebot_plugin_autoreply-0.2.8/nonebot_plugin_autoreply/util.py` & `nonebot_plugin_autoreply-0.2.9/nonebot_plugin_autoreply/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Any, Dict, Tuple, Union, cast
 
+from anyio import Path
+from nonebot.adapters.onebot.utils import f2s
 from nonebot.adapters.onebot.v11 import (
     Bot,
     GroupMessageEvent,
     Message,
     MessageEvent,
     MessageSegment,
     PokeNotifyEvent,
@@ -53,21 +55,26 @@
     seg_var = {
         "at": MessageSegment.at(user_id),
         "reply": MessageSegment.reply(message_id) if message_id else None,
     }
     return normal_var, seg_var
 
 
-def replace_message_var(message: Message, var_dict: VarDictType) -> Message:
+async def replace_message_var(message: Message, var_dict: VarDictType) -> Message:
     normal_var, seg_var = var_dict
     message = cast(
         Message,
         Message.template(message).format_map({**normal_var, **seg_var}),
     )
 
     for seg in message:
         if not seg.is_text():
             for k, v in seg.data.items():
                 if isinstance(v, str):
                     seg.data[k] = v.format(**normal_var)
 
+        if seg.type in ("image", "record"):
+            file = seg.data.get("file")
+            if isinstance(file, str) and file.startswith("file:///"):
+                seg.data["file"] = f2s(await Path(file[8:]).read_bytes())
+
     return message
```

### Comparing `nonebot_plugin_autoreply-0.2.8/pyproject.toml` & `nonebot_plugin_autoreply-0.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [project]
 name = "nonebot-plugin-autoreply"
-version = "0.2.8"
+version = "0.2.9"
 description = "A powerful auto reply plugin for NoneBot2"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc1",
     "pydantic>=1.10.4",
     "nonebot-adapter-onebot>=2.1.0",
     "typing-extensions>=4.4.0",
     "PyYAML>=6.0",
+    "anyio>=3.6.2",
 ]
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

