# Comparing `tmp/nonebot_plugin_memes-0.4.6.tar.gz` & `tmp/nonebot_plugin_memes-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_memes-0.4.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_memes-0.4.7.tar", max compression
```

## Comparing `nonebot_plugin_memes-0.4.6.tar` & `nonebot_plugin_memes-0.4.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/LICENSE
--rw-r--r--   0        0        0     6459 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/README.md
--rw-r--r--   0        0        0    14799 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/__init__.py
--rw-r--r--   0        0        0      523 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/config.py
--rw-r--r--   0        0        0      152 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/data_source/__init__.py
--rw-r--r--   0        0        0     2857 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/data_source/image_source.py
--rw-r--r--   0        0        0      375 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/data_source/user_id.py
--rw-r--r--   0        0        0     1978 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/data_source/user_info.py
--rw-r--r--   0        0        0     7507 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/depends.py
--rw-r--r--   0        0        0      155 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/exception.py
--rw-r--r--   0        0        0     4858 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/manager.py
--rw-r--r--   0        0        0     3135 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/rule.py
--rw-r--r--   0        0        0     2561 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/utils.py
--rw-r--r--   0        0        0      752 2023-04-29 06:11:31.403272 nonebot_plugin_memes-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     7471 1970-01-01 00:00:00.000000 nonebot_plugin_memes-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-21 05:38:39.010329 nonebot_plugin_memes-0.4.7/LICENSE
+-rw-r--r--   0        0        0     6459 2023-07-21 05:38:39.010329 nonebot_plugin_memes-0.4.7/README.md
+-rw-r--r--   0        0        0    14972 2023-07-21 05:38:39.010329 nonebot_plugin_memes-0.4.7/nonebot_plugin_memes/__init__.py
+-rw-r--r--   0        0        0      523 2023-07-21 05:38:39.010329 nonebot_plugin_memes-0.4.7/nonebot_plugin_memes/config.py
+-rw-r--r--   0        0        0      152 2023-07-21 05:38:39.010329 nonebot_plugin_memes-0.4.7/nonebot_plugin_memes/data_source/__init__.py
+-rw-r--r--   0        0        0     2857 2023-07-21 05:38:39.010329 nonebot_plugin_memes-0.4.7/nonebot_plugin_memes/data_source/image_source.py
+-rw-r--r--   0        0        0      375 2023-07-21 05:38:39.010329 nonebot_plugin_memes-0.4.7/nonebot_plugin_memes/data_source/user_id.py
+-rw-r--r--   0        0        0     1978 2023-07-21 05:38:39.010329 nonebot_plugin_memes-0.4.7/nonebot_plugin_memes/data_source/user_info.py
+-rw-r--r--   0        0        0     7507 2023-07-21 05:38:39.010329 nonebot_plugin_memes-0.4.7/nonebot_plugin_memes/depends.py
+-rw-r--r--   0        0        0      155 2023-07-21 05:38:39.010329 nonebot_plugin_memes-0.4.7/nonebot_plugin_memes/exception.py
+-rw-r--r--   0        0        0     4858 2023-07-21 05:38:39.010329 nonebot_plugin_memes-0.4.7/nonebot_plugin_memes/manager.py
+-rw-r--r--   0        0        0     3135 2023-07-21 05:38:39.010329 nonebot_plugin_memes-0.4.7/nonebot_plugin_memes/rule.py
+-rw-r--r--   0        0        0     2561 2023-07-21 05:38:39.014329 nonebot_plugin_memes-0.4.7/nonebot_plugin_memes/utils.py
+-rw-r--r--   0        0        0      747 2023-07-21 05:38:39.014329 nonebot_plugin_memes-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     7466 1970-01-01 00:00:00.000000 nonebot_plugin_memes-0.4.7/PKG-INFO
```

### Comparing `nonebot_plugin_memes-0.4.6/LICENSE` & `nonebot_plugin_memes-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes-0.4.6/README.md` & `nonebot_plugin_memes-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/__init__.py` & `nonebot_plugin_memes-0.4.7/nonebot_plugin_memes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 from nonebot.utils import run_sync
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
@@ -60,18 +60,22 @@
 from .rule import command_rule, regex_rule
 from .utils import meme_info
 
 __plugin_meta__ = PluginMetadata(
     name="表情包制作",
     description="制作各种沙雕表情包",
     usage="发送“表情包制作”查看表情包列表",
+    type="application",
+    homepage="https://github.com/noneplugin/nonebot-plugin-memes",
+    config=Config,
+    supported_adapters={"~onebot.v11", "~onebot.v12"},
     extra={
         "unique_name": "memes",
         "author": "meetwq <meetwq@gmail.com>",
-        "version": "0.4.6",
+        "version": "0.4.7",
     },
 )
 
 memes_cache_dir = get_cache_dir("nonebot_plugin_memes")
 
 
 PERM_EDIT = GROUP_ADMIN | GROUP_OWNER | PRIVATE_FRIEND | PRIVATE | SUPERUSER
```

### Comparing `nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/config.py` & `nonebot_plugin_memes-0.4.7/nonebot_plugin_memes/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/data_source/image_source.py` & `nonebot_plugin_memes-0.4.7/nonebot_plugin_memes/data_source/image_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/data_source/user_info.py` & `nonebot_plugin_memes-0.4.7/nonebot_plugin_memes/data_source/user_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/depends.py` & `nonebot_plugin_memes-0.4.7/nonebot_plugin_memes/depends.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/manager.py` & `nonebot_plugin_memes-0.4.7/nonebot_plugin_memes/manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/rule.py` & `nonebot_plugin_memes-0.4.7/nonebot_plugin_memes/rule.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/utils.py` & `nonebot_plugin_memes-0.4.7/nonebot_plugin_memes/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes-0.4.6/pyproject.toml` & `nonebot_plugin_memes-0.4.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "nonebot_plugin_memes"
-version = "0.4.6"
+version = "0.4.7"
 description = "Nonebot2 plugin for making memes"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-memes"
 repository = "https://github.com/noneplugin/nonebot-plugin-memes"
 
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
-pil-utils = "^0.1.4"
+pil-utils = "^0.1.7"
 meme-generator = ">=0.0.7,<0.1.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `nonebot_plugin_memes-0.4.6/PKG-INFO` & `nonebot_plugin_memes-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-memes
-Version: 0.4.6
+Version: 0.4.7
 Summary: Nonebot2 plugin for making memes
 Home-page: https://github.com/noneplugin/nonebot-plugin-memes
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
 Requires-Dist: meme-generator (>=0.0.7,<0.1.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0)
-Requires-Dist: nonebot-plugin-localstore (>=0.4.0,<0.5.0)
-Requires-Dist: nonebot2[fastapi] (>=2.0.0-rc.1,<3.0.0)
-Requires-Dist: pil-utils (>=0.1.4,<0.2.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
+Requires-Dist: nonebot-plugin-localstore (>=0.5.0,<0.6.0)
+Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
+Requires-Dist: pil-utils (>=0.1.7,<0.2.0)
 Requires-Dist: pypinyin (>=0.44.0,<1.0.0)
 Project-URL: Repository, https://github.com/noneplugin/nonebot-plugin-memes
 Description-Content-Type: text/markdown
 
 <div align="center">
 
   <a href="https://v2.nonebot.dev/">
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-memes Version: 0.4.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-memes Version: 0.4.7 Summary:
 Nonebot2 plugin for making memes Home-page: https://github.com/noneplugin/
 nonebot-plugin-memes License: MIT Author: meetwq Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-
 Dist: meme-generator (>=0.0.7,<0.1.0) Requires-Dist: nonebot-adapter-onebot
-(>=2.2.2,<3.0.0) Requires-Dist: nonebot-plugin-localstore (>=0.4.0,<0.5.0)
-Requires-Dist: nonebot2[fastapi] (>=2.0.0-rc.1,<3.0.0) Requires-Dist: pil-utils
-(>=0.1.4,<0.2.0) Requires-Dist: pypinyin (>=0.44.0,<1.0.0) Project-URL:
+(>=2.2.3,<3.0.0) Requires-Dist: nonebot-plugin-localstore (>=0.5.0,<0.6.0)
+Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0) Requires-Dist: pil-utils
+(>=0.1.7,<0.2.0) Requires-Dist: pypinyin (>=0.44.0,<1.0.0) Project-URL:
 Repository, https://github.com/noneplugin/nonebot-plugin-memes Description-
 Content-Type: text/markdown
  [nonebot] # nonebot-plugin-memes _â¨ [Nonebot2](https://github.com/nonebot/
                      nonebot2) è¡¨æåå¶ä½æä»¶ â¨_
                 [license] [Python] [NoneBot] [pypi] [qq_group]
 > æ¬æä»¶ v0.4.x çæ¬ä¸ºå [å¤´åè¡¨æå](https://github.com/
 noneplugin/nonebot-plugin-petpet) ä¸ [æå­è¡¨æå](https://github.com/
```

