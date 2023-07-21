# Comparing `tmp/nonebot_plugin_ncm-1.5.5.tar.gz` & `tmp/nonebot_plugin_ncm-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ncm-1.5.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_ncm-1.6.0.tar", max compression
```

## Comparing `nonebot_plugin_ncm-1.5.5.tar` & `nonebot_plugin_ncm-1.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-03-04 16:08:48.835826 nonebot_plugin_ncm-1.5.5/LICENSE
--rw-r--r--   0        0        0     3451 2023-03-04 16:08:48.835826 nonebot_plugin_ncm-1.5.5/README.md
--rw-r--r--   0        0        0    13255 2023-03-04 16:08:48.835826 nonebot_plugin_ncm-1.5.5/nonebot-plugin-ncm/__init__.py
--rw-r--r--   0        0        0      627 2023-03-04 16:08:48.835826 nonebot_plugin_ncm-1.5.5/nonebot-plugin-ncm/config.py
--rw-r--r--   0        0        0    12469 2023-03-04 16:08:48.835826 nonebot_plugin_ncm-1.5.5/nonebot-plugin-ncm/data_source.py
--rw-r--r--   0        0        0      859 2023-03-04 16:08:48.835826 nonebot_plugin_ncm-1.5.5/pyproject.toml
--rw-r--r--   0        0        0     4608 1970-01-01 00:00:00.000000 nonebot_plugin_ncm-1.5.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-21 14:51:11.583203 nonebot_plugin_ncm-1.6.0/LICENSE
+-rw-r--r--   0        0        0     4733 2023-07-21 14:51:11.583203 nonebot_plugin_ncm-1.6.0/README.md
+-rw-r--r--   0        0        0    14172 2023-07-21 14:51:11.583203 nonebot_plugin_ncm-1.6.0/nonebot-plugin-ncm/__init__.py
+-rw-r--r--   0        0        0      734 2023-07-21 14:51:11.583203 nonebot_plugin_ncm-1.6.0/nonebot-plugin-ncm/config.py
+-rw-r--r--   0        0        0    12800 2023-07-21 14:51:11.583203 nonebot_plugin_ncm-1.6.0/nonebot-plugin-ncm/data_source.py
+-rw-r--r--   0        0        0      859 2023-07-21 14:51:11.583203 nonebot_plugin_ncm-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5890 1970-01-01 00:00:00.000000 nonebot_plugin_ncm-1.6.0/PKG-INFO
```

### Comparing `nonebot_plugin_ncm-1.5.5/LICENSE` & `nonebot_plugin_ncm-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ncm-1.5.5/nonebot-plugin-ncm/__init__.py` & `nonebot_plugin_ncm-1.6.0/nonebot-plugin-ncm/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,62 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+from dataclasses import dataclass
 from pathlib import Path
-from typing import Tuple, Any, Union
+from typing import Tuple, Any, Union, Optional, Type, Set, Dict
 
 import nonebot
 from nonebot import on_regex, on_command, on_message
 from nonebot.adapters.onebot.v11 import (Message, Bot,
                                          MessageSegment,
                                          GroupMessageEvent,
                                          PrivateMessageEvent)
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg, RegexGroup, Arg
 from nonebot.rule import Rule
+from pydantic.main import BaseModel
 
 from .data_source import nncm, ncm_config, setting, Q, cmd
 
+
 # =======nonebot-plugin-help=======
-__plugin_meta__ = nonebot.plugin.PluginMetadata(
-    name='网易云无损音乐下载',
-    description='✨ 基于go-cqhttp与nonebot2的 网易云 无损音乐下载 ✨',
-    usage=(
+@dataclass(eq=False)
+class PluginMetadata:
+    """插件元信息，由插件编写者提供"""
+
+    name: str = "网易云无损音乐下载",
+    """插件名称"""
+    description: str = "✨ 基于go-cqhttp与nonebot2的 网易云 无损音乐下载 ✨",
+    """插件功能介绍"""
+    usage: str = (
         '将网易云歌曲/歌单分享到群聊即可自动解析\n'
         '回复分享消息 + 文字`下载` 即可开始下载歌曲并上传到群文件(需要稍等一会)\n'
         '指令：\n'
         f'开启下载：{cmd}ncm t\n'
         f'关闭下载：{cmd}ncm f\n'
         f'点歌：{cmd}点歌 歌名'
-    ),
-    extra={'version': '1.5.0'}
-)
+    )
+    """插件使用方法"""
+    type: Optional[str] = "application"
+    """插件类型，用于商店分类"""
+    homepage: Optional[str] = "https://github.com/kitUIN/nonebot-plugin-ncm"
+    """插件主页"""
+    config: Optional[Type[BaseModel]] = ncm_config
+    """插件配置项"""
+    supported_adapters: Optional[Set[str]] = {"nonebot.adapters.onebot.v11"},
+    """插件支持的适配器模块路径
+
+    格式为 `<module>[:<Adapter>]`，`~` 为 `nonebot.adapters.` 的缩写。
+
+    `None` 表示支持**所有适配器**。
+    """
+
 
+__plugin_meta__ = PluginMetadata(...)
 # ========nonebot-plugin-ncm======
 # ===========Constant=============
 TRUE = ["True", "T", "true", "t"]
 FALSE = ["False", "F", "false", "f"]
 ADMIN = ["owner", "admin", "member"]
 
 
@@ -120,15 +142,14 @@
 
 
 @search.got("song", prompt="要点什么歌捏?")
 async def receive_song(bot: Bot,
                        event: Union[GroupMessageEvent, PrivateMessageEvent],
                        song: Message = Arg(),
                        ):
-    nncm.get_session(bot, event)
     _id = await nncm.search_song(keyword=str(song), limit=1)
     message_id = await bot.send(event=event, message=Message(MessageSegment.music(type_="163", id_=_id)))
     nncm.get_song(message_id=message_id["message_id"], nid=_id)
     # try:
 
     # except ActionFailed as e:
     #    logger.error(e.info)
@@ -136,66 +157,64 @@
 
 
 @music_regex.handle()
 async def music_receive(bot: Bot, event: Union[GroupMessageEvent, PrivateMessageEvent],
                         regroup: Tuple[Any, ...] = RegexGroup()):
     nid = regroup[1]
     logger.info(f"已识别NID:{nid}的歌曲")
-    nncm.get_session(bot, event)
-    nncm.get_song(nid)
+    nncm.get_song(nid=nid, message_id=event.message_id)
 
 
 @playlist_regex.handle()
 async def music_list_receive(bot: Bot, event: Union[GroupMessageEvent, PrivateMessageEvent],
                              regroup: Tuple[Any, ...] = RegexGroup()):
     lid = regroup[0]
     logger.info(f"已识别LID:{lid}的歌单")
-    nncm.get_session(bot, event)
-    nncm.get_playlist(lid=lid)
+    nncm.get_playlist(lid=lid, message_id=event.message_id)
 
 
 @music_reply.handle()
 async def music_reply_receive(bot: Bot, event: Union[GroupMessageEvent, PrivateMessageEvent]):
-    # logger.info(event.dict()["reply"]["message_id"])
-    nncm.get_session(bot, event)
-    info = nncm.check_message()
+    info = nncm.check_message(int(event.dict()["reply"]["message_id"]))
     if info is None:
         return
     if info["type"] == "song" and await song_is_open(event):
         await bot.send(event=event, message="少女祈祷中🙏...上传时间较久,请勿重复发送命令")
-        await nncm.download(ids=[int(info["nid"])])
         data = await nncm.music_check(info["nid"])
+        if isinstance(data, list):
+            data = data[0]
         if data:
             if isinstance(event, GroupMessageEvent):
-                await nncm.upload_group_data_file(data)
+                await nncm.upload_group_data_file(event.group_id, data)
             elif isinstance(event, PrivateMessageEvent):
-                await nncm.upload_private_data_file(data)
+                await nncm.upload_private_data_file(event.user_id, data)
         else:
             logger.error("数据库中未有该音乐地址数据")
+            await bot.send(event=event, message="数据库中未有该音乐地址数据")
 
     elif info["type"] == "playlist" and await playlist_is_open(event):
-        await bot.send(event=event, message=info["lmsg"]+"\n下载中,上传时间较久,请勿重复发送命令")
+        await bot.send(event=event, message=info["lmsg"] + "\n下载中,上传时间较久,请勿重复发送命令")
         not_zips = await nncm.download(ids=info["ids"], lid=info["lid"], is_zip=ncm_config.ncm_playlist_zip)
         filename = f"{info['lid']}.zip"
         data = Path.cwd().joinpath("music").joinpath(filename)
         if ncm_config.ncm_playlist_zip:
             logger.debug(f"Upload:{filename}")
             if isinstance(event, GroupMessageEvent):
-                await nncm.upload_group_file(file=str(data), name=filename)
+                await nncm.upload_group_file(group_id=event.group_id, file=str(data), name=filename)
             elif isinstance(event, PrivateMessageEvent):
-                await nncm.upload_private_file(file=str(data), name=filename)
+                await nncm.upload_private_file(user_id=event.user_id, file=str(data), name=filename)
         else:
             for i in not_zips:
                 file = i["file"]
                 filename = i["filename"]
                 logger.debug(f"Upload:{filename}")
                 if isinstance(event, GroupMessageEvent):
-                    await nncm.upload_group_file(file=file, name=filename)
+                    await nncm.upload_group_file(group_id=event.group_id, file=file, name=filename)
                 elif isinstance(event, PrivateMessageEvent):
-                    await nncm.upload_private_file(file=file, name=filename)
+                    await nncm.upload_private_file(user_id=event.user_id, file=file, name=filename)
 
 
 @ncm_set.handle()
 async def set_receive(bot: Bot, event: Union[GroupMessageEvent, PrivateMessageEvent],
                       args: Message = CommandArg()):  # 功能设置接收
     logger.debug(f"权限为{event.sender.role}的用户<{event.sender.nickname}>尝试使用命令{cmd}ncm {args}")
     if args:
```

### Comparing `nonebot_plugin_ncm-1.5.5/nonebot-plugin-ncm/config.py` & `nonebot_plugin_ncm-1.6.0/nonebot-plugin-ncm/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,11 +16,13 @@
     '''手机号区域码,默认86'''
 
     ncm_password: str = ""
     '''密码'''
 
     ncm_playlist_zip: bool = False
     '''上传歌单时是否压缩'''
+    ncm_bitrate: int = 320
+    '''下载码率(单位K) 96及以下为m4a,320及以上为flac,中间mp3'''
 
 
 global_config = nonebot.get_driver().config
 ncm_config = Config(**global_config.dict())  # 载入配置
```

### Comparing `nonebot_plugin_ncm-1.5.5/nonebot-plugin-ncm/data_source.py` & `nonebot_plugin_ncm-1.6.0/nonebot-plugin-ncm/data_source.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import os
 import zipfile
 from pathlib import Path
 from datetime import datetime
-from typing import Union
+from typing import Union, List, Optional, Dict
 import re
 
 import qrcode
 import time
 from aiofile import async_open
 
 import httpx
@@ -47,50 +47,47 @@
 class NcmLoginFailedException(Exception): pass
 
 
 # ============主类=============
 class Ncm:
     def __init__(self):
         self.api = apis
-        self.bot = None
-        self.event = None
-
-    def get_session(self, bot: Bot, event: Union[GroupMessageEvent, PrivateMessageEvent]):
-        self.bot = bot
-        self.event = event
 
     @staticmethod
     def save_user(session: str):
         info = ncm_user_cache.search(Q["uid"] == "user")
         if info:
             info[0]['session'] = session
             ncm_user_cache.update(info[0], Q["uid"] == "user")
         else:
             ncm_user_cache.insert({"uid": "user", "session": session})
 
     @staticmethod
-    def load_user(info):
-        SetCurrentSession(LoadSessionFromString(info[0]['session']))
+    def load_user(session: str):
+        SetCurrentSession(LoadSessionFromString(session))
 
-    def login(self):
+    def login(self) -> bool:
         try:
             self.api.login.LoginViaCellphone(phone=ncm_config.ncm_phone, password=ncm_config.ncm_password)
             self.get_user_info()
-
+            return True
         except Exception as e:
             if str(e) == str({'code': 400, 'message': '登陆失败,请进行安全验证'}):
                 logger.error("缺少安全验证，请将账号留空进行二维码登录")
                 logger.info("自动切换为二维码登录↓")
                 self.get_qrcode()
             else:
                 raise e
+            return False
 
-    def get_user_info(self):
-        logger.success(f"欢迎您网易云用户:{GetCurrentSession().nickname} [{GetCurrentSession().uid}]")
+    def get_user_info(self) -> str:
+        message: str = f"欢迎您网易云用户:{GetCurrentSession().nickname} [{GetCurrentSession().uid}]";
+        logger.success(message)
         self.save_user(DumpSessionAsString(GetCurrentSession()))
+        return message
 
     def get_phone_login(self):
         phone = ncm_config.ncm_phone
         ctcode = int(ncm_config.ncm_ctcode)
         result = self.api.login.SetSendRegisterVerifcationCodeViaCellphone(cell=phone, ctcode=ctcode)
         if not result.get('code', 0) == 200:
             logger.error(result)
@@ -130,25 +127,22 @@
             time.sleep(1)
 
     def detail(self, ids: list) -> list:
         songs: list = self.api.track.GetTrackDetail(song_ids=ids)["songs"]
         detail = [(data["name"] + "-" + ",".join([names["name"] for names in data["ar"]])) for data in songs]
         return detail
 
-    async def music_check(self, nid):
+    async def music_check(self, nid: int) -> Union[List[Dict[str, Union[str, int]]], Dict[str, Union[str, int]], None]:
         nid = int(nid)
         info = music.search(Q["id"] == nid)
         if info:
             path = Path(info[0]["file"])
             if path.is_file():
                 return info[0]
-            else:
-                return await self.download(ids=[nid], check=True)
-        else:
-            return None
+        return await self.download(ids=[nid])
 
     async def search_song(self, keyword: str, limit: int = 1) -> int:  # 搜索歌曲
         res = self.api.cloudsearch.GetSearchResult(keyword=keyword, stype=SONG, limit=limit)
         logger.debug(f"搜索歌曲{keyword},返回结果:{res}")
         if "result" in res.keys():
             data = res["result"]["songs"]
         else:
@@ -158,105 +152,111 @@
 
     async def search_user(self, keyword: str, limit: int = 1):  # 搜索用户
         self.api.cloudsearch.GetSearchResult(keyword=keyword, stype=USER, limit=limit)
 
     async def search_playlist(self, keyword: str, limit: int = 1):  # 搜索歌单
         self.api.cloudsearch.GetSearchResult(keyword=keyword, stype=PLAYLIST, limit=limit)
 
-    def check_message(self):
+    @staticmethod
+    def check_message(message_id: int):
         """检查缓存中是否存在解析
         :return:
         """
-        info = ncm_check_cache.search(Q.message_id == self.event.dict()["reply"]["message_id"])
+        info = ncm_check_cache.search(Q.message_id == message_id)
         return info[0] if info else None
 
-    def get_song(self, nid: Union[int, str], message_id=None):
+    @staticmethod
+    def get_song(nid: int, message_id: int):
         """解析歌曲id,并且加入缓存
 
         :param message_id:
         :param nid:
         :return:
         """
-        if message_id:
-            mid = message_id
-        else:
-            mid = self.event.message_id
-        ncm_check_cache.insert({"message_id": mid,
+        ncm_check_cache.insert({"message_id": message_id,
                                 "type": "song",
-                                "nid": nid,
+                                "nid": int(nid),
                                 "lid": 0,
                                 "ids": [],
                                 "lmsg": "",
                                 "time": int(time.time())})
 
-    def get_playlist(self, lid: Union[int, str]):
+    def get_playlist(self, lid: int, message_id: int):
+        lid = int(lid)
         data = self.api.playlist.GetPlaylistInfo(lid)
         # logger.info(data)
         if data["code"] == 200:
             raw = data["playlist"]
             tags = ",".join(raw['tags'])
-            songs = [i['id'] for i in raw['trackIds']]
-            ncm_check_cache.insert({"message_id": self.event.message_id,
+            songs = [int(i['id']) for i in raw['trackIds']]
+            ncm_check_cache.insert({"message_id": message_id,
                                     "type": "playlist",
                                     "nid": 0,
                                     "lid": lid,
                                     "ids": songs,
                                     "lmsg": f"歌单:{raw['name']}\r\n创建者:{raw['creator']['nickname']}\r\n歌曲总数:{raw['trackCount']}\r\n"
                                             f"标签:{tags}\r\n播放次数:{raw['playCount']}\r\n收藏:{raw['subscribedCount']}\r\n"
                                             f"评论:{raw['commentCount']}\r\n分享:{raw['shareCount']}\r\nListID:{lid}",
                                     "time": int(time.time())})
 
-    async def upload_group_data_file(self, data):
-        await self.upload_group_file(file=data["file"], name=data["filename"])
+    async def upload_group_data_file(self, group_id: int, data: Dict[str, Union[str, int]]):
+        await self.upload_group_file(group_id=group_id, file=data["file"], name=data["filename"])
 
-    async def upload_private_data_file(self, data):
-        await self.upload_private_file(file=data["file"], name=data["filename"])
+    async def upload_private_data_file(self, user_id: int, data: Dict[str, Union[str, int]]):
+        await self.upload_private_file(user_id=user_id, file=data["file"], name=data["filename"])
 
-    async def upload_group_file(self, file, name):
+    @staticmethod
+    async def upload_group_file(group_id: int, file: str, name: str):
         try:
-            await self.bot.upload_group_file(group_id=self.event.group_id,
-                                             file=file, name=name)
+            bot: Bot = nonebot.get_bot()
+            await bot.upload_group_file(group_id=group_id, file=file, name=name)
         except (ActionFailed, NetworkError) as e:
             logger.error(e)
+            bot: Bot = nonebot.get_bot()
             if isinstance(e, ActionFailed) and e.info["wording"] == "server" \
                                                                     " requires unsupported ftn upload":
-                await self.bot.send(event=self.event, message=Message(MessageSegment.text(
+                await bot.send_group_msg(group_id=group_id, message=Message(MessageSegment.text(
                     "[ERROR]  文件上传失败\r\n[原因]  机器人缺少上传文件的权限\r\n[解决办法]  "
                     "请将机器人设置为管理员或者允许群员上传文件")))
             elif isinstance(e, NetworkError):
-                await self.bot.send(event=self.event, message=Message(MessageSegment.text("[ERROR]文件上传失败\r\n[原因]  "
-                                                                                          "上传超时(一般来说还在传,建议等待五分钟)")))
+                await bot.send_group_msg(group_id=group_id,
+                                         message=Message(MessageSegment.text("[ERROR]文件上传失败\r\n[原因]  "
+                                                                             "上传超时(一般来说还在传,建议等待五分钟)")))
 
-    async def upload_private_file(self, file, name):
+    @staticmethod
+    async def upload_private_file(user_id: int, file: str, name: str):
         try:
-            await self.bot.upload_private_file(user_id=self.event.user_id,
-                                               file=file, name=name)
+            bot: Bot = nonebot.get_bot()
+            await bot.upload_private_file(user_id=user_id, file=file, name=name)
         except (ActionFailed, NetworkError) as e:
             logger.error(e)
             if isinstance(e, NetworkError):
-                await self.bot.send(event=self.event, message=Message(MessageSegment.text(
+                bot: Bot = nonebot.get_bot()
+                await  bot.send_private_msg(user_id=user_id, message=Message(MessageSegment.text(
                     "[ERROR]  文件上传失败\r\n[原因]  上传超时(一般来说还在传,建议等待五分钟)")))
 
     @run_sync
-    def get_zip(self, lid, filenames: list):
+    def get_zip(self, lid: int, filenames: list):
         zip_file_new = f'{lid}.zip'
         with zipfile.ZipFile(str(Path.cwd().joinpath("music").joinpath(zip_file_new)), 'w', zipfile.ZIP_DEFLATED) as z:
             for f in filenames:
                 z.write(str(f), f.name)
         return zip_file_new
 
-    async def download(self, ids: list, check=False, lid=0, is_zip=False):  # 下载音乐
-        data: list = self.api.track.GetTrackAudio(song_ids=ids, bitrate=3200 * 1000)["data"]
+    async def download(self, ids: List[int], lid: int = 0, is_zip=False) -> Optional[List[Dict[str, Union[str, int]]]]:
+        """一般地 320k及以上即 flac, 320k及以下即 mp3,96k及以下即 m4a
+        """
+        data: list = self.api.track.GetTrackAudio(song_ids=ids, bitrate=ncm_config.ncm_bitrate * 1000)["data"]
         name: list = self.detail(ids)
         filenames = []
         not_zips = []
         for i in range(len(ids)):
             if data[i]["code"] == 404:
                 logger.error("未从网易云读取到下载地址")
-                return
+                return None
             url = data[i]["url"]
             nid = data[i]["id"]
             filename = f"{name[i]}.{data[i]['type']}"
             filename = re.sub('[\/:*?"<>|]', '-', filename)
             file = Path.cwd().joinpath("music").joinpath(filename)
             config = {
                 "id": int(nid),
@@ -283,15 +283,15 @@
         return not_zips
 
 
 nncm = Ncm()
 info = ncm_user_cache.search(Q.uid == "user")
 if info:
     logger.info("检测到缓存，自动加载用户")
-    nncm.load_user(info)
+    nncm.load_user(info[0]['session'])
     nncm.get_user_info()
 elif ncm_config.ncm_phone == "":
     logger.warning("您未填写账号,自动进入二维码登录模式")
     nncm.get_qrcode()
 elif ncm_config.ncm_password == "":
     logger.warning("您未填写密码,自动进入手机验证码登录模式")
     nncm.get_phone_login()
```

### Comparing `nonebot_plugin_ncm-1.5.5/pyproject.toml` & `nonebot_plugin_ncm-1.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-ncm"
-version = "1.5.5"
+version = "1.6.0"
 description = "基于go-cqhttp与nonebot2的 网易云 无损音乐下载"
 license = "Apache License 2.0"
 authors = ["kitUIN <kulujun@gmail.com>"]
 maintainers = ["kitUIN <kulujun@gmail.com>", "Kurokitu"]
 readme = "README.md"
 packages = [
     { include = "nonebot-plugin-ncm" }
@@ -12,16 +12,16 @@
 homepage = "https://github.com/kitUIN/nonebot-plugin-ncm"
 repository = "https://github.com/kitUIN/nonebot-plugin-ncm"
 keywords = ["netease-cloud-music", "netease", "go-cqhttp", "nonebot2"]
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = "^2.0.0rc2"
 tinydb = "^4.7.0"
-pyncm ="^1.6.8.3"
-aiofile ="^3.7.4"
+pyncm ="^1.6.9.1"
+aiofile ="^3.8.7"
 nonebot-adapter-onebot = "^2.1.5"
 qrcode = "^7.3.1"
 httpx = "^0.23.1"
 Pillow = "^9.3.0"
 [tool.poetry.dev-dependencies]
 
 [build-system]
```

### Comparing `nonebot_plugin_ncm-1.5.5/PKG-INFO` & `nonebot_plugin_ncm-1.6.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-ncm
-Version: 1.5.5
-Summary: 基于go-cqhttp与nonebot2的 网易云 无损音乐下载
-Home-page: https://github.com/kitUIN/nonebot-plugin-ncm
-License: Apache-2.0
-Keywords: netease-cloud-music,netease,go-cqhttp,nonebot2
-Author: kitUIN
-Author-email: kulujun@gmail.com
-Maintainer: kitUIN
-Maintainer-email: kulujun@gmail.com
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Pillow (>=9.3.0,<10.0.0)
-Requires-Dist: aiofile (>=3.7.4,<4.0.0)
-Requires-Dist: httpx (>=0.23.1,<0.24.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.1.5,<3.0.0)
-Requires-Dist: nonebot2 (>=2.0.0rc2,<3.0.0)
-Requires-Dist: pyncm (>=1.6.8.3,<2.0.0.0)
-Requires-Dist: qrcode (>=7.3.1,<8.0.0)
-Requires-Dist: tinydb (>=4.7.0,<5.0.0)
-Project-URL: Repository, https://github.com/kitUIN/nonebot-plugin-ncm
-Description-Content-Type: text/markdown
-
 
 
 <p align="center">
   <img src="https://files.catbox.moe/7cy61g.png" width="200" height="200" alt="nonebot"></a>
 </p>
 
 <div align="center">
@@ -53,70 +24,110 @@
   <a href="https://github.com/kitUIN/nonebot-plugin-ncm/releases">
     <img src="https://img.shields.io/github/v/release/kitUIN/nonebot-plugin-ncm" alt="release">
   </a>
   <a href="https://wakatime.com/badge/user/3b5608c7-e0b6-44a2-a217-cad786040b48/project/2a431792-e82f-48f5-839c-9ee566910fe5"><img src="https://wakatime.com/badge/user/3b5608c7-e0b6-44a2-a217-cad786040b48/project/2a431792-e82f-48f5-839c-9ee566910fe5.svg" alt="wakatime"></a>
 </p>
 
 
-## 安装
-### 使用pip安装
-1.`pip install nonebot-plugin-ncm` 进行安装  
-2.并在`bot.py`添加`nonebot.load_plugin('nonebot-plugin-ncm')`
-### 使用nb-cli安装(推荐)
-`nb plugin install nonebot-plugin-ncm` 进行安装
+## 安装 💿
+ 
+<details>
+<summary>使用 nb-cli 安装</summary>
+在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
+
+    nb plugin install nonebot-plugin-ncm  
+    或者  
+    python -m nb_cli plugin install nonebot-plugin-ncm  
+    
+</details>
 
 <details>
+<summary>使用包管理器安装</summary>
+在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
+
+<details>
+<summary>pip</summary>
+
+    pip install nonebot-plugin-ncm
+</details>
+<details>
+<summary>pdm</summary>
+
+    pdm add nonebot-plugin-ncm
+</details>
+<details>
+<summary>poetry</summary>
+
+    poetry add nonebot-plugin-ncm
+</details>
+
+打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
+
+    plugins = ["nonebot-plugin-ncm"]
+
+</details>
+<details>
   <summary>如果希望使用`nonebot2 a16`及以下版本 </summary>
-  请使用`pip install nonebot-plugin-ncm==1.1.0`进行安装
+  
+    pip install nonebot-plugin-ncm==1.1.0
 </details>
 
-## 升级
-1.`pip install nonebot-plugin-ncm --upgrade` 进行升级  
-2. 低于`1.5.0`版本升级请删除`db`文件夹内`ncm`开头文件  
-3. 根据新的`config`项配置`.env`文件
-## 快速使用
+## 快速使用 ▶️
 将链接或者卡片分享到聊天群或机器人,回复分享的消息并输入`下载`即可进行下载  
-**默认下载状态为关闭，请在每个群内使用`/ncm t`开启,私聊则默认开启**
-![img](https://files.catbox.moe/g7c230.png)
-### 命令列表：
+分享之后是没有反应的,只有对需要解析的消息回复`下载`才会响应  
+**默认下载状态为关闭，请在每个群内使用`/ncm t`开启,私聊则默认开启**  
+![a1v9gk.png](https://files.catbox.moe/a1v9gk.png)
+
+
+## 注意说明 ⚠️
+- 使用的网易云账号**需要拥有黑胶VIP** 
+- 默认下载最高音质的音乐,可以修改`ncm_bitrate`项更改音乐品质  
+- 本程序实质为调用web接口下载音乐上传
+
+### 命令列表 📃
 | 命令                 | 备注        |
 |--------------------|-----------|
 | /ncm               | 获取命令菜单    |
 | /ncm t             | 开启下载      |
 | /ncm f             | 关闭下载      |
 | /ncm search t      | 开启点歌      |
 | /ncm search f      | 关闭点歌      |
 | /点歌 歌名             | 点歌        |
 | /ncm private qq号 t | 开启该用户私聊下载 |
 | /ncm private qq号 f | 关闭该用户私聊下载 |
 - 命令开始符号会自动识别[`COMMAND_START`](https://v2.nonebot.dev/docs/api/config#Config-command_start)项
 
-## 注意说明
-- 使用的网易云账号**需要拥有黑胶VIP** 
-- 默认下载最高音质的音乐 
-- 本程序实质为调用web接口下载音乐上传  
 
-## 配置文件说明
+## 配置文件说明 ⚙️
+| 配置项 | 必填 | 默认值 | 说明 |
+|:-----:|:----:|:----:|:----:|
+| ncm_admin_level | 否 | 1 | 设置命令权限(1:仅限superusers和群主,2:在1的基础上+管理员,3:所有用户) |
+| ncm_ctcode | 否 | 86 | 手机号区域码 |
+| ncm_phone | 是 |   | 网易云绑定的手机号(留空则二维码登录) |
+| ncm_password | 是 |   | 网易云账号密码(留空则短信登录) |
+| ncm_playlist_zip | 否 | False | 是否开启本地图片存储，True为开启本地图片存储 |
+| ncm_bitrate | 否 | 320 | 下载码率(单位K) <=96: m4a, >=320:flac, 96< mp3 <320|
 ```
+# 这是示例
 ncm_admin_level=1 # 设置命令权限(1:仅限superusers和群主,2:在1的基础上+管理员,3:所有用户)
 ncm_ctcode="86" # 手机号区域码,默认86
 ncm_phone=  # 手机登录
 ncm_password=  # 密码
 ncm_playlist_zip=False # 上传歌单时是否压缩
+ncm_bitrate: int = 320 # 下载码率(单位K) 96及以下为m4a,320及以上为flac,中间mp3
 ```
 
-## 功能列表
+## 功能列表 📃
 - [x] 识别/下载 网易云单曲
     - 链接
     - 卡片
     - 卡片转发
 - [x] 识别/下载 网易云歌单    
     - 链接
     - 卡片
     - 卡片转发
 - [x] 点歌(网易云)
 - [ ] QQ音乐无损下载
 
 # 鸣谢
 - [pyncm](https://github.com/greats3an/pyncm)
 - [nonebot2](https://github.com/nonebot/nonebot2)
-
```

#### html2text {}

```diff
@@ -1,49 +1,46 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-ncm Version: 1.5.5 Summary:
-åºäºgo-cqhttpä¸nonebot2ç ç½æäº æ æé³ä¹ä¸è½½ Home-page: https://
-github.com/kitUIN/nonebot-plugin-ncm License: Apache-2.0 Keywords: netease-
-cloud-music,netease,go-cqhttp,nonebot2 Author: kitUIN Author-email:
-kulujun@gmail.com Maintainer: kitUIN Maintainer-email: kulujun@gmail.com
-Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: Apache
-Software License Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Dist: Pillow (>=9.3.0,<10.0.0)
-Requires-Dist: aiofile (>=3.7.4,<4.0.0) Requires-Dist: httpx (>=0.23.1,<0.24.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.1.5,<3.0.0) Requires-Dist: nonebot2
-(>=2.0.0rc2,<3.0.0) Requires-Dist: pyncm (>=1.6.8.3,<2.0.0.0) Requires-Dist:
-qrcode (>=7.3.1,<8.0.0) Requires-Dist: tinydb (>=4.7.0,<5.0.0) Project-URL:
-Repository, https://github.com/kitUIN/nonebot-plugin-ncm Description-Content-
-Type: text/markdown
                                    [nonebot]
  # nonebot-plugin-ncm â¨ åºäºgo-cqhttpä¸nonebot2ç ç½æäº æ æé³ä¹
                                ç¹æ­/ä¸è½½ â¨
                 [license] [pypi] [nonebot] [release] [wakatime]
-## å®è£ ### ä½¿ç¨pipå®è£ 1.`pip install nonebot-plugin-ncm` è¿è¡å®è£
-2.å¹¶å¨`bot.py`æ·»å `nonebot.load_plugin('nonebot-plugin-ncm')` ### ä½¿ç¨nb-
-cliå®è£(æ¨è) `nb plugin install nonebot-plugin-ncm` è¿è¡å®è£
-å¦æå¸æä½¿ç¨`nonebot2 a16`åä»¥ä¸çæ¬  è¯·ä½¿ç¨`pip install nonebot-
-plugin-ncm==1.1.0`è¿è¡å®è£  ## åçº§ 1.`pip install nonebot-plugin-ncm --
-upgrade` è¿è¡åçº§ 2.
-ä½äº`1.5.0`çæ¬åçº§è¯·å é¤`db`æä»¶å¤¹å`ncm`å¼å¤´æä»¶ 3.
-æ ¹æ®æ°ç`config`é¡¹éç½®`.env`æä»¶ ## å¿«éä½¿ç¨
+## å®è£ ð¿  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
+install nonebot-plugin-ncm æè python -m nb_cli plugin install nonebot-
+plugin-ncm   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
+æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
+pip pip install nonebot-plugin-ncm   pdm pdm add nonebot-plugin-ncm   poetry
+poetry add nonebot-plugin-ncm  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
+`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
+["nonebot-plugin-ncm"]   å¦æå¸æä½¿ç¨`nonebot2 a16`åä»¥ä¸çæ¬  pip
+install nonebot-plugin-ncm==1.1.0  ## å¿«éä½¿ç¨ â¶ï¸
 å°é¾æ¥æèå¡çåäº«å°èå¤©ç¾¤ææºå¨äºº,åå¤åäº«çæ¶æ¯å¹¶è¾å¥`ä¸è½½`å³å¯è¿è¡ä¸è½½
+åäº«ä¹åæ¯æ²¡æååºç,åªæå¯¹éè¦è§£æçæ¶æ¯åå¤`ä¸è½½`æä¼ååº
 **é»è®¤ä¸è½½ç¶æä¸ºå³é­ï¼è¯·å¨æ¯ä¸ªç¾¤åä½¿ç¨`/ncm
-t`å¼å¯,ç§èåé»è®¤å¼å¯** ![img](https://files.catbox.moe/g7c230.png)
-### å½ä»¤åè¡¨ï¼ | å½ä»¤ | å¤æ³¨ | |--------------------|-----------| | /
-ncm | è·åå½ä»¤èå | | /ncm t | å¼å¯ä¸è½½ | | /ncm f | å³é­ä¸è½½ |
-| /ncm search t | å¼å¯ç¹æ­ | | /ncm search f | å³é­ç¹æ­ | | /ç¹æ­
-æ­å | ç¹æ­ | | /ncm private qqå· t | å¼å¯è¯¥ç¨æ·ç§èä¸è½½ | | /ncm
-private qqå· f | å³é­è¯¥ç¨æ·ç§èä¸è½½ | -
-å½ä»¤å¼å§ç¬¦å·ä¼èªå¨è¯å«[`COMMAND_START`](https://v2.nonebot.dev/docs/
-api/config#Config-command_start)é¡¹ ## æ³¨æè¯´æ -
+t`å¼å¯,ç§èåé»è®¤å¼å¯** ![a1v9gk.png](https://files.catbox.moe/
+a1v9gk.png) ## æ³¨æè¯´æ â ï¸ -
 ä½¿ç¨çç½æäºè´¦å·**éè¦æ¥æé»è¶VIP** -
-é»è®¤ä¸è½½æé«é³è´¨çé³ä¹ -
-æ¬ç¨åºå®è´¨ä¸ºè°ç¨webæ¥å£ä¸è½½é³ä¹ä¸ä¼  ## éç½®æä»¶è¯´æ ```
-ncm_admin_level=1 # è®¾ç½®å½ä»¤æé(1:ä»ésuperusersåç¾¤ä¸»,2:
-å¨1çåºç¡ä¸+ç®¡çå,3:ææç¨æ·) ncm_ctcode="86" #
-ææºå·åºåç ,é»è®¤86 ncm_phone= # ææºç»å½ ncm_password= # å¯ç 
-ncm_playlist_zip=False # ä¸ä¼ æ­åæ¶æ¯å¦åç¼© ``` ## åè½åè¡¨ - [x]
+é»è®¤ä¸è½½æé«é³è´¨çé³ä¹,å¯ä»¥ä¿®æ¹`ncm_bitrate`é¡¹æ´æ¹é³ä¹åè´¨
+- æ¬ç¨åºå®è´¨ä¸ºè°ç¨webæ¥å£ä¸è½½é³ä¹ä¸ä¼  ### å½ä»¤åè¡¨ ð |
+å½ä»¤ | å¤æ³¨ | |--------------------|-----------| | /ncm |
+è·åå½ä»¤èå | | /ncm t | å¼å¯ä¸è½½ | | /ncm f | å³é­ä¸è½½ | | /ncm
+search t | å¼å¯ç¹æ­ | | /ncm search f | å³é­ç¹æ­ | | /ç¹æ­ æ­å |
+ç¹æ­ | | /ncm private qqå· t | å¼å¯è¯¥ç¨æ·ç§èä¸è½½ | | /ncm private
+qqå· f | å³é­è¯¥ç¨æ·ç§èä¸è½½ | - å½ä»¤å¼å§ç¬¦å·ä¼èªå¨è¯å«
+[`COMMAND_START`](https://v2.nonebot.dev/docs/api/config#Config-
+command_start)é¡¹ ## éç½®æä»¶è¯´æ âï¸ | éç½®é¡¹ | å¿å¡« | é»è®¤å¼
+| è¯´æ | |:-----:|:----:|:----:|:----:| | ncm_admin_level | å¦ | 1 |
+è®¾ç½®å½ä»¤æé(1:ä»ésuperusersåç¾¤ä¸»,2:å¨1çåºç¡ä¸+ç®¡çå,3:
+ææç¨æ·) | | ncm_ctcode | å¦ | 86 | ææºå·åºåç  | | ncm_phone |
+æ¯ | | ç½æäºç»å®çææºå·(çç©ºåäºç»´ç ç»å½) | | ncm_password
+| æ¯ | | ç½æäºè´¦å·å¯ç (çç©ºåç­ä¿¡ç»å½) | | ncm_playlist_zip |
+å¦ | False | æ¯å¦å¼å¯æ¬å°å¾çå­å¨ï¼Trueä¸ºå¼å¯æ¬å°å¾çå­å¨
+| | ncm_bitrate | å¦ | 320 | ä¸è½½ç ç(åä½K) <=96: m4a, >=320:flac, 96<
+mp3 <320| ``` # è¿æ¯ç¤ºä¾ ncm_admin_level=1 # è®¾ç½®å½ä»¤æé(1:
+ä»ésuperusersåç¾¤ä¸»,2:å¨1çåºç¡ä¸+ç®¡çå,3:ææç¨æ·)
+ncm_ctcode="86" # ææºå·åºåç ,é»è®¤86 ncm_phone= # ææºç»å½
+ncm_password= # å¯ç  ncm_playlist_zip=False # ä¸ä¼ æ­åæ¶æ¯å¦åç¼©
+ncm_bitrate: int = 320 # ä¸è½½ç ç(åä½K)
+96åä»¥ä¸ä¸ºm4a,320åä»¥ä¸ä¸ºflac,ä¸­é´mp3 ``` ## åè½åè¡¨ ð - [x]
 è¯å«/ä¸è½½ ç½æäºåæ² - é¾æ¥ - å¡ç - å¡çè½¬å - [x] è¯å«/
 ä¸è½½ ç½æäºæ­å - é¾æ¥ - å¡ç - å¡çè½¬å - [x] ç¹æ­(ç½æäº)
 - [ ] QQé³ä¹æ æä¸è½½ # é¸£è°¢ - [pyncm](https://github.com/greats3an/
 pyncm) - [nonebot2](https://github.com/nonebot/nonebot2)
```

