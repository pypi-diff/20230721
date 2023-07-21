# Comparing `tmp/nonebot_plugin_eventmonitor-0.1.6.tar.gz` & `tmp/nonebot_plugin_eventmonitor-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_eventmonitor-0.1.6.tar", last modified: Sun Apr 16 07:21:47 2023, max compression
+gzip compressed data, was "nonebot_plugin_eventmonitor-0.1.7.tar", last modified: Fri Jul 21 15:08:47 2023, max compression
```

## Comparing `nonebot_plugin_eventmonitor-0.1.6.tar` & `nonebot_plugin_eventmonitor-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 07:21:47.476523 nonebot_plugin_eventmonitor-0.1.6/
--rw-rw-rw-   0        0        0    35149 2023-01-29 04:13:58.000000 nonebot_plugin_eventmonitor-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     1320 2023-04-16 07:21:47.460916 nonebot_plugin_eventmonitor-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      689 2023-04-16 07:19:49.000000 nonebot_plugin_eventmonitor-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 07:21:47.414026 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor/
--rw-rw-rw-   0        0        0     4627 2023-04-09 06:00:28.000000 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor/__init__.py
--rw-rw-rw-   0        0        0     1882 2023-04-09 05:58:13.000000 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor/admin.py
--rw-rw-rw-   0        0        0     1086 2023-04-16 07:03:41.000000 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor/honour.py
--rw-rw-rw-   0        0        0     1995 2023-04-09 05:58:48.000000 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor/stamp.py
--rw-rw-rw-   0        0        0      386 2023-04-16 07:04:11.000000 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:21:47.460916 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor.egg-info/
--rw-rw-rw-   0        0        0     1320 2023-04-16 07:21:46.000000 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      469 2023-04-16 07:21:47.000000 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 07:21:46.000000 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-16 07:21:46.000000 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-04-16 07:21:46.000000 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 07:21:47.476523 nonebot_plugin_eventmonitor-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      993 2023-04-16 07:11:29.000000 nonebot_plugin_eventmonitor-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 15:08:47.975588 nonebot_plugin_eventmonitor-0.1.7/
+-rw-rw-rw-   0        0        0    35149 2023-01-29 04:13:58.000000 nonebot_plugin_eventmonitor-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     1478 2023-07-21 15:08:47.975588 nonebot_plugin_eventmonitor-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2023-07-21 15:01:10.000000 nonebot_plugin_eventmonitor-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 15:08:47.944874 nonebot_plugin_eventmonitor-0.1.7/nonebot_plugin_eventmonitor/
+-rw-rw-rw-   0        0        0     7158 2023-07-21 15:03:44.000000 nonebot_plugin_eventmonitor-0.1.7/nonebot_plugin_eventmonitor/__init__.py
+-rw-rw-rw-   0        0        0     1878 2023-07-21 09:06:43.000000 nonebot_plugin_eventmonitor-0.1.7/nonebot_plugin_eventmonitor/admin.py
+-rw-rw-rw-   0        0        0     1088 2023-07-21 09:06:47.000000 nonebot_plugin_eventmonitor-0.1.7/nonebot_plugin_eventmonitor/honour.py
+-rw-rw-rw-   0        0        0     2018 2023-07-21 14:45:01.000000 nonebot_plugin_eventmonitor-0.1.7/nonebot_plugin_eventmonitor/stamp.py
+-rw-rw-rw-   0        0        0     4903 2023-07-21 14:52:24.000000 nonebot_plugin_eventmonitor-0.1.7/nonebot_plugin_eventmonitor/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 15:08:47.974591 nonebot_plugin_eventmonitor-0.1.7/nonebot_plugin_eventmonitor.egg-info/
+-rw-rw-rw-   0        0        0     1478 2023-07-21 15:08:47.000000 nonebot_plugin_eventmonitor-0.1.7/nonebot_plugin_eventmonitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2023-07-21 15:08:47.000000 nonebot_plugin_eventmonitor-0.1.7/nonebot_plugin_eventmonitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 15:08:47.000000 nonebot_plugin_eventmonitor-0.1.7/nonebot_plugin_eventmonitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-21 15:08:47.000000 nonebot_plugin_eventmonitor-0.1.7/nonebot_plugin_eventmonitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-21 15:08:47.000000 nonebot_plugin_eventmonitor-0.1.7/nonebot_plugin_eventmonitor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 15:08:47.976587 nonebot_plugin_eventmonitor-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      993 2023-07-21 15:07:31.000000 nonebot_plugin_eventmonitor-0.1.7/setup.py
```

### Comparing `nonebot_plugin_eventmonitor-0.1.6/LICENSE` & `nonebot_plugin_eventmonitor-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_eventmonitor-0.1.6/PKG-INFO` & `nonebot_plugin_eventmonitor-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_eventmonitor
-Version: 0.1.6
+Version: 0.1.7
 Summary: 监控群事件的插件，支持戳一戳，成员变动，群荣誉，运气王变化等提示
 Home-page: https://github.com/Reversedeer/nonebot_plugin_eventmonitor
 Author: schwarzwald
 Project-URL: Bug Tracker, https://github.com/Reversedeer/nonebot_plugin_eventmonitor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <details>
     <summary><h2>更新日志</h2></summary>
 
-- v0.1.6
+- v0.1.7
 
+  - 新增所有功能开关[#issue5](https://github.com/Reversedeer/nonebot_plugin_eventmonitor/issues/9
+  - 增加权限控制
+  - 修复潜在的bug
+- v0.1.6
   - 修复bug
-  
 - v0.1.5
-  - 优化配置文件 [#issue6](https://github.com/Reversedeer/nonebot_plugin_eventmonitor/issues/6)
+  - 优化配置文件 [#issue4](https://github.com/Reversedeer/nonebot_plugin_eventmonitor/issues/6
   - 删除冗余代码
   - 修复获取superusers数值bug
-
 - v0.1.3
   - 修复配置文件bug
 - v0.1.2
   - 增加了戳一戳的文案
 
   - 修改一些bug
 - v0.1.1
```

### Comparing `nonebot_plugin_eventmonitor-0.1.6/README.md` & `nonebot_plugin_eventmonitor-0.1.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 <details>
     <summary><h2>更新日志</h2></summary>
 
-- v0.1.6
+- v0.1.7
 
+  - 新增所有功能开关[#issue5](https://github.com/Reversedeer/nonebot_plugin_eventmonitor/issues/9
+  - 增加权限控制
+  - 修复潜在的bug
+- v0.1.6
   - 修复bug
-  
 - v0.1.5
-  - 优化配置文件 [#issue6](https://github.com/Reversedeer/nonebot_plugin_eventmonitor/issues/6)
+  - 优化配置文件 [#issue4](https://github.com/Reversedeer/nonebot_plugin_eventmonitor/issues/6
   - 删除冗余代码
   - 修复获取superusers数值bug
-
 - v0.1.3
   - 修复配置文件bug
 - v0.1.2
   - 增加了戳一戳的文案
 
   - 修改一些bug
 - v0.1.1
```

### Comparing `nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor/admin.py` & `nonebot_plugin_eventmonitor-0.1.7/nonebot_plugin_eventmonitor/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,27 +15,25 @@
         admin_msg = (
             "呜呜，别下咱管理呀QwQ，喵呜~"
             if user_id == bot_qq
             else f"🚔 管理员变动\n[CQ:at,qq={user_id}]痛失本群管理喵~"
         )
     return admin_msg
 
-
 async def del_user_bye(add_time, user_id):
     global del_user_msg
     del_time = datetime.fromtimestamp(add_time)
     if user_id in superusers:
         del_user_msg = f"⌈{del_time}⌋\n@{user_id}恭送主人离开喵~"
         print(superusers)
     else:
         del_user_msg = f"✈️ 成员变动⌈{del_time}⌋\nQQ号为：{user_id}的小可爱退群喵~" \
                        f"[CQ:image,file=https://q4.qlogo.cn/headimg_dl?dst_uin={user_id}&spec=640]"
         return del_user_msg
 
-
 async def add_user_wecome(add_time, user_id, bot_qq):
     global groups_all, add_user_msg
     add_time = datetime.fromtimestamp(add_time)
     if user_id == bot_qq:
         add_user_msg = f"本喵被邀进入贵群喵~\n" \
                        f"火速上个管理喵~"
     elif user_id in superusers:
```

### Comparing `nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor/honour.py` & `nonebot_plugin_eventmonitor-0.1.7/nonebot_plugin_eventmonitor/honour.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .utils import superusers
 
+
 async def monitor_rongyu(honor_type, user_id, bot_qq):  
     rely = ""
 
     if honor_type == "emotion":
         if user_id == bot_qq:
             pass
         elif user_id in superusers:
```

### Comparing `nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor/stamp.py` & `nonebot_plugin_eventmonitor-0.1.7/nonebot_plugin_eventmonitor/stamp.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,11 +47,9 @@
     "(。´・ω・)ん?",
     "有事恁叫我，别天天一个劲戳戳戳！",
     "欸很烦欸！你戳🔨呢",
     "再戳一下试试？",
     "正在关闭对您的所有服务...关闭成功",
     "啊呜，太舒服刚刚竟然睡着了。什么事？",
     "正在定位您的真实地址...定位成功。轰炸机已起飞"
+    "再戳就更大了qwq"
 ]
-
-
-
```

### Comparing `nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor.egg-info/PKG-INFO` & `nonebot_plugin_eventmonitor-0.1.7/nonebot_plugin_eventmonitor.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-eventmonitor
-Version: 0.1.6
+Version: 0.1.7
 Summary: 监控群事件的插件，支持戳一戳，成员变动，群荣誉，运气王变化等提示
 Home-page: https://github.com/Reversedeer/nonebot_plugin_eventmonitor
 Author: schwarzwald
 Project-URL: Bug Tracker, https://github.com/Reversedeer/nonebot_plugin_eventmonitor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <details>
     <summary><h2>更新日志</h2></summary>
 
-- v0.1.6
+- v0.1.7
 
+  - 新增所有功能开关[#issue5](https://github.com/Reversedeer/nonebot_plugin_eventmonitor/issues/9
+  - 增加权限控制
+  - 修复潜在的bug
+- v0.1.6
   - 修复bug
-  
 - v0.1.5
-  - 优化配置文件 [#issue6](https://github.com/Reversedeer/nonebot_plugin_eventmonitor/issues/6)
+  - 优化配置文件 [#issue4](https://github.com/Reversedeer/nonebot_plugin_eventmonitor/issues/6
   - 删除冗余代码
   - 修复获取superusers数值bug
-
 - v0.1.3
   - 修复配置文件bug
 - v0.1.2
   - 增加了戳一戳的文案
 
   - 修改一些bug
 - v0.1.1
```

### Comparing `nonebot_plugin_eventmonitor-0.1.6/setup.py` & `nonebot_plugin_eventmonitor-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot_plugin_eventmonitor",
-    version="0.1.6",
+    version="0.1.7",
     author="schwarzwald",
     description="监控群事件的插件，支持戳一戳，成员变动，群荣誉，运气王变化等提示",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Reversedeer/nonebot_plugin_eventmonitor",
     project_urls={
         "Bug Tracker": "https://github.com/Reversedeer/nonebot_plugin_eventmonitor/issues",
```

