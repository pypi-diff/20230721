# Comparing `tmp/nonebot_plugin_groupmate_waifu-1.2.8.tar.gz` & `tmp/nonebot_plugin_groupmate_waifu-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_groupmate_waifu-1.2.8.tar", last modified: Tue Jul 18 10:16:48 2023, max compression
+gzip compressed data, was "nonebot_plugin_groupmate_waifu-1.2.9.tar", last modified: Fri Jul 21 12:57:26 2023, max compression
```

## Comparing `nonebot_plugin_groupmate_waifu-1.2.8.tar` & `nonebot_plugin_groupmate_waifu-1.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 10:16:48.119390 nonebot_plugin_groupmate_waifu-1.2.8/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_groupmate_waifu-1.2.8/LICENSE
--rw-rw-rw-   0        0        0      279 2023-07-18 10:16:48.117889 nonebot_plugin_groupmate_waifu-1.2.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 10:16:48.106958 nonebot_plugin_groupmate_waifu-1.2.8/nonebot_plugin_groupmate_waifu/
--rw-rw-rw-   0        0        0    21797 2023-07-18 10:14:30.000000 nonebot_plugin_groupmate_waifu-1.2.8/nonebot_plugin_groupmate_waifu/__init__.py
--rw-rw-rw-   0        0        0      354 2023-07-17 15:11:43.000000 nonebot_plugin_groupmate_waifu-1.2.8/nonebot_plugin_groupmate_waifu/config.py
--rw-rw-rw-   0        0        0     2090 2023-07-17 13:11:31.000000 nonebot_plugin_groupmate_waifu-1.2.8/nonebot_plugin_groupmate_waifu/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-18 10:16:48.116388 nonebot_plugin_groupmate_waifu-1.2.8/nonebot_plugin_groupmate_waifu.egg-info/
--rw-rw-rw-   0        0        0      279 2023-07-18 10:16:47.000000 nonebot_plugin_groupmate_waifu-1.2.8/nonebot_plugin_groupmate_waifu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-07-18 10:16:48.000000 nonebot_plugin_groupmate_waifu-1.2.8/nonebot_plugin_groupmate_waifu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 10:16:47.000000 nonebot_plugin_groupmate_waifu-1.2.8/nonebot_plugin_groupmate_waifu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-07-18 10:16:47.000000 nonebot_plugin_groupmate_waifu-1.2.8/nonebot_plugin_groupmate_waifu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-07-18 10:16:47.000000 nonebot_plugin_groupmate_waifu-1.2.8/nonebot_plugin_groupmate_waifu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 10:16:48.119390 nonebot_plugin_groupmate_waifu-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      583 2023-07-18 10:16:42.000000 nonebot_plugin_groupmate_waifu-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:57:26.346466 nonebot_plugin_groupmate_waifu-1.2.9/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_groupmate_waifu-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0      279 2023-07-21 12:57:26.345965 nonebot_plugin_groupmate_waifu-1.2.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-21 12:57:26.332747 nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu/
+-rw-rw-rw-   0        0        0    21887 2023-07-21 12:53:08.000000 nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu/__init__.py
+-rw-rw-rw-   0        0        0      354 2023-07-17 15:11:43.000000 nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu/config.py
+-rw-rw-rw-   0        0        0     2015 2023-07-21 12:53:08.000000 nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:57:26.344463 nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-07-21 12:57:26.000000 nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-07-21 12:57:26.000000 nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 12:57:26.000000 nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-07-21 12:57:26.000000 nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-07-21 12:57:26.000000 nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 12:57:26.346966 nonebot_plugin_groupmate_waifu-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      567 2023-07-21 12:57:21.000000 nonebot_plugin_groupmate_waifu-1.2.9/setup.py
```

### Comparing `nonebot_plugin_groupmate_waifu-1.2.8/LICENSE` & `nonebot_plugin_groupmate_waifu-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_groupmate_waifu-1.2.8/nonebot_plugin_groupmate_waifu/__init__.py` & `nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from nonebot import require
 from nonebot.plugin.on import on_command,on_message
 from nonebot.permission import SUPERUSER
 from nonebot.typing import T_State
 from nonebot.adapters.onebot.v11 import (
-    GROUP,
     GROUP_ADMIN,
     GROUP_OWNER,
     Bot,
     GroupMessageEvent,
     Message,
     MessageSegment,
     )
@@ -16,19 +15,14 @@
 import os
 import random
 import asyncio
 import time
 
 from pathlib import Path
 
-try:
-    import ujson as json
-except ModuleNotFoundError:
-    import json
-
 from .utils import *
 from .config import Config
 
 from nonebot.plugin import PluginMetadata
 
 __plugin_meta__ = PluginMetadata(
     name = "娶群友",
@@ -125,32 +119,35 @@
         record_lock = {}
     if record_yinpa1_file.exists() and os.path.getmtime(record_yinpa1_file) > Zero_today:
         record_yinpa1 = {}
     if record_yinpa2_file.exists() and os.path.getmtime(record_yinpa2_file) > Zero_today:
         record_yinpa2 = {}
 
     # 重置记录
-    @scheduler.scheduled_job("cron",hour = 0, misfire_grace_time = 120)
-    def _():
-        global record_CP,record_yinpa1,record_yinpa2
+    def reset_record():
+        global record_CP,record_waifu,record_lock,record_yinpa1,record_yinpa2
         record_CP = {}
+        record_waifu = {}
+        record_lock = {}
         record_yinpa1 = {}
         record_yinpa2 = {}
 else:
     # 重置记录
-    @scheduler.scheduled_job("cron",hour = 0, misfire_grace_time = 120)
-    def _():
+    def reset_record():
         global record_CP,record_yinpa1,record_yinpa2
         for group_id in record_CP:
             for user_id in record_CP[group_id]:
                 if record_CP[group_id][user_id] == user_id:
                     record_CP[group_id][user_id] = 0
         record_yinpa1 = {}
         record_yinpa2 = {}
 
+on_command("重置记录", priority = 80, block = True).append_handler(reset_record)
+scheduler.add_job(reset_record,"cron",hour = 0, misfire_grace_time = 120)
+
 protect_list_file = waifu_file / "list_protect"
 if protect_list_file.exists():
     with open(protect_list_file,'r') as f:
         line = f.read()
         protect_list = eval(line)
 else:
     protect_list = {}
@@ -271,21 +268,22 @@
                     msg = "你已经有CP了，不许花心哦~" + MessageSegment.image(file = await user_img(waifu_id)) + f"你的CP：{member['card'] or member['nickname']}"
             else:
                 msg = tips + MessageSegment.image(file = await user_img(waifu_id)) + f"『{member['card'] or member['nickname']}』！"
             await bot.send(event,msg,at_sender = True)
             return False
 
     if at:
+        tips = "恭喜你娶到了群友!\n" + tips
         if at == rec.get(at):
             waifu_id = at
+            del rec[waifu_id]
         else:
             X = random.randint(1,100)
             if 0 < X <= HE:
                 waifu_id = at
-                tips = "恭喜你娶到了群友!\n" + tips
             elif HE < X <= BE:
                 waifu_id = user_id
     if not waifu_id:
         group_id = event.group_id
         member_list = await bot.get_group_member_list(group_id = group_id)
         lastmonth = event.time - last_sent_time_filter
         id_list = {member['user_id'] for member in member_list if member["last_sent_time"] > lastmonth}
@@ -342,15 +340,15 @@
 if waifu_cd_bye > -1:
     global cd_bye
     cd_bye = {}
 
     bye = on_command(
         "离婚",
         aliases = {"分手"},
-        rule = lambda event:event.group_id in record_CP and record_CP[event.group_id].get(event.user_id,event.user_id) != event.user_id,
+        rule = lambda event:isinstance(event,GroupMessageEvent) and event.group_id in record_CP and record_CP[event.group_id].get(event.user_id,event.user_id) != event.user_id,
         priority = 90,
         block = True
         )
     @bye.handle()
     async def _(event: GroupMessageEvent):
         group_id = event.group_id
         user_id = event.user_id
```

### Comparing `nonebot_plugin_groupmate_waifu-1.2.8/nonebot_plugin_groupmate_waifu/utils.py` & `nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,14 @@
 import httpx
 import hashlib
 import asyncio
 
 from pil_utils import BuildImage,Text2Image
 from nonebot.adapters.onebot.v11 import Message
 
-try:
-    import ujson as json
-except ModuleNotFoundError:
-    import json
-
 async def download_avatar(user_id: int) -> bytes:
     url = f"https://q1.qlogo.cn/g?b=qq&nk={user_id}&s=640"
     data = await download_url(url)
     if hashlib.md5(data).hexdigest() == "acef72340ac0e914090bd35799f5594e":
         url = f"https://q1.qlogo.cn/g?b=qq&nk={user_id}&s=100"
         data = await download_url(url)
     return data
```

### Comparing `nonebot_plugin_groupmate_waifu-1.2.8/setup.py` & `nonebot_plugin_groupmate_waifu-1.2.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_groupmate_waifu',
-version='1.2.8',
+version='1.2.9',
 description='娶群友',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_groupmate_waifu"]),
 platforms='all',
-install_requires=["nonebot2","nonebot-adapter-onebot","nonebot_plugin_apscheduler","nonebot_plugin_imageutils"],
+install_requires=["nonebot2","nonebot-adapter-onebot","nonebot_plugin_apscheduler","pil_utils"],
 url='https://github.com/KarisAya/nonebot_plugin_groupmate_waifu',
 )
```

