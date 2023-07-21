# Comparing `tmp/nonebot_plugin_memes_api-0.1.4.tar.gz` & `tmp/nonebot_plugin_memes_api-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_memes_api-0.1.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_memes_api-0.1.5.tar", max compression
```

## Comparing `nonebot_plugin_memes_api-0.1.4.tar` & `nonebot_plugin_memes_api-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1063 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/LICENSE
--rw-r--r--   0        0        0     3310 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/README.md
--rw-r--r--   0        0        0    15014 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/__init__.py
--rw-r--r--   0        0        0      532 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/config.py
--rw-r--r--   0        0        0      152 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/data_source/__init__.py
--rw-r--r--   0        0        0     2857 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/data_source/image_source.py
--rw-r--r--   0        0        0      375 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/data_source/user_id.py
--rw-r--r--   0        0        0     1978 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/data_source/user_info.py
--rw-r--r--   0        0        0     7468 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/depends.py
--rw-r--r--   0        0        0      967 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/exception.py
--rw-r--r--   0        0        0     5047 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/manager.py
--rw-r--r--   0        0        0     4999 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/request.py
--rw-r--r--   0        0        0     3135 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/rule.py
--rw-r--r--   0        0        0     2415 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/utils.py
--rw-r--r--   0        0        0      709 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4245 1970-01-01 00:00:00.000000 nonebot_plugin_memes_api-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-21 06:38:57.632841 nonebot_plugin_memes_api-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3310 2023-07-21 06:38:57.632841 nonebot_plugin_memes_api-0.1.5/README.md
+-rw-r--r--   0        0        0    15191 2023-07-21 06:38:57.632841 nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/__init__.py
+-rw-r--r--   0        0        0      532 2023-07-21 06:38:57.632841 nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/config.py
+-rw-r--r--   0        0        0      152 2023-07-21 06:38:57.632841 nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/data_source/__init__.py
+-rw-r--r--   0        0        0     2857 2023-07-21 06:38:57.632841 nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/data_source/image_source.py
+-rw-r--r--   0        0        0      375 2023-07-21 06:38:57.632841 nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/data_source/user_id.py
+-rw-r--r--   0        0        0     1978 2023-07-21 06:38:57.632841 nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/data_source/user_info.py
+-rw-r--r--   0        0        0     7468 2023-07-21 06:38:57.632841 nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/depends.py
+-rw-r--r--   0        0        0      967 2023-07-21 06:38:57.632841 nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/exception.py
+-rw-r--r--   0        0        0     5047 2023-07-21 06:38:57.632841 nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/manager.py
+-rw-r--r--   0        0        0     4999 2023-07-21 06:38:57.632841 nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/request.py
+-rw-r--r--   0        0        0     3135 2023-07-21 06:38:57.632841 nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/rule.py
+-rw-r--r--   0        0        0     2415 2023-07-21 06:38:57.632841 nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/utils.py
+-rw-r--r--   0        0        0      704 2023-07-21 06:38:57.632841 nonebot_plugin_memes_api-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4240 1970-01-01 00:00:00.000000 nonebot_plugin_memes_api-0.1.5/PKG-INFO
```

### Comparing `nonebot_plugin_memes_api-0.1.4/LICENSE` & `nonebot_plugin_memes_api-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes_api-0.1.4/README.md` & `nonebot_plugin_memes_api-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/__init__.py` & `nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from nonebot.typing import T_Handler, T_State
 from pypinyin import Style, pinyin
 
 require("nonebot_plugin_localstore")
 
 from nonebot_plugin_localstore import get_cache_dir
 
-from .config import memes_config
+from .config import Config, memes_config
 from .data_source import ImageSource, User, UserInfo
 from .depends import (
     IMAGE_SOURCES_KEY,
     TEXTS_KEY,
     USERS_KEY,
     split_msg_v11,
     split_msg_v12,
@@ -59,18 +59,22 @@
 from .rule import command_rule, regex_rule
 from .utils import meme_info
 
 __plugin_meta__ = PluginMetadata(
     name="表情包制作",
     description="制作各种沙雕表情包",
     usage="发送“表情包制作”查看表情包列表",
+    type="application",
+    homepage="https://github.com/noneplugin/nonebot-plugin-memes-api",
+    config=Config,
+    supported_adapters={"~onebot.v11", "~onebot.v12"},
     extra={
         "unique_name": "memes_api",
         "author": "meetwq <meetwq@gmail.com>",
-        "version": "0.1.4",
+        "version": "0.1.5",
     },
 )
 
 memes_cache_dir = get_cache_dir("nonebot_plugin_memes_api")
 
 
 PERM_EDIT = GROUP_ADMIN | GROUP_OWNER | PRIVATE_FRIEND | PRIVATE | SUPERUSER
```

### Comparing `nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/config.py` & `nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/data_source/image_source.py` & `nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/data_source/image_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/data_source/user_info.py` & `nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/data_source/user_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/depends.py` & `nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/depends.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/exception.py` & `nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/manager.py` & `nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/request.py` & `nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/rule.py` & `nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/rule.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/utils.py` & `nonebot_plugin_memes_api-0.1.5/nonebot_plugin_memes_api/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes_api-0.1.4/pyproject.toml` & `nonebot_plugin_memes_api-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "nonebot_plugin_memes_api"
-version = "0.1.4"
+version = "0.1.5"
 description = "Nonebot2 plugin for making memes"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-memes-api"
 repository = "https://github.com/noneplugin/nonebot-plugin-memes-api"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = { version = "^2.0.0-rc.1", extras = ["fastapi"] }
-nonebot-adapter-onebot = "^2.2.2"
-nonebot-plugin-localstore = "^0.4.0"
+nonebot2 = { version = "^2.0.0", extras = ["fastapi"] }
+nonebot-adapter-onebot = "^2.2.3"
+nonebot-plugin-localstore = "^0.5.0"
 httpx = ">=0.20.0,<1.0.0"
 pypinyin = ">=0.44.0,<1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.1.0"
 
 [build-system]
```

### Comparing `nonebot_plugin_memes_api-0.1.4/PKG-INFO` & `nonebot_plugin_memes_api-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-memes-api
-Version: 0.1.4
+Version: 0.1.5
 Summary: Nonebot2 plugin for making memes
 Home-page: https://github.com/noneplugin/nonebot-plugin-memes-api
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.20.0,<1.0.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0)
-Requires-Dist: nonebot-plugin-localstore (>=0.4.0,<0.5.0)
-Requires-Dist: nonebot2[fastapi] (>=2.0.0-rc.1,<3.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
+Requires-Dist: nonebot-plugin-localstore (>=0.5.0,<0.6.0)
+Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
 Requires-Dist: pypinyin (>=0.44.0,<1.0.0)
 Project-URL: Repository, https://github.com/noneplugin/nonebot-plugin-memes-api
 Description-Content-Type: text/markdown
 
 <div align="center">
 
   <a href="https://v2.nonebot.dev/">
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-memes-api Version: 0.1.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-memes-api Version: 0.1.5 Summary:
 Nonebot2 plugin for making memes Home-page: https://github.com/noneplugin/
 nonebot-plugin-memes-api License: MIT Author: meetwq Author-email:
 meetwq@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: httpx
-(>=0.20.0,<1.0.0) Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0)
-Requires-Dist: nonebot-plugin-localstore (>=0.4.0,<0.5.0) Requires-Dist:
-nonebot2[fastapi] (>=2.0.0-rc.1,<3.0.0) Requires-Dist: pypinyin
-(>=0.44.0,<1.0.0) Project-URL: Repository, https://github.com/noneplugin/
-nonebot-plugin-memes-api Description-Content-Type: text/markdown
+(>=0.20.0,<1.0.0) Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
+Requires-Dist: nonebot-plugin-localstore (>=0.5.0,<0.6.0) Requires-Dist:
+nonebot2[fastapi] (>=2.0.0,<3.0.0) Requires-Dist: pypinyin (>=0.44.0,<1.0.0)
+Project-URL: Repository, https://github.com/noneplugin/nonebot-plugin-memes-api
+Description-Content-Type: text/markdown
    [nonebot] # nonebot-plugin-memes-api _â¨ [Nonebot2](https://github.com/
         nonebot/nonebot2) è¡¨æåå¶ä½æä»¶ è°ç¨ api çæ¬ â¨_
                 [license] [Python] [NoneBot] [pypi] [qq_group]
 > æ¬æä»¶ä¸º [nonebot-plugin-memes](https://github.com/noneplugin/nonebot-
 plugin-memes) è°ç¨ api çæ¬ > > å¯ä»¥å°æ¬æä»¶ä¸ [meme-generator]
 (https://github.com/MeetWq/meme-generator) åå¼é¨ç½² ### å®è£ - ä½¿ç¨ nb-
 cli ``` nb plugin install nonebot_plugin_memes_api ``` - ä½¿ç¨ pip ``` pip
```

