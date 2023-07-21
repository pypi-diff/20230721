# Comparing `tmp/nonebot_plugin_stable_diffusion_diao-0.3.9.5.6.tar.gz` & `tmp/nonebot_plugin_stable_diffusion_diao-0.3.9.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.9.5.6.tar", last modified: Thu Jul 20 14:40:36 2023, max compression
+gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.9.5.7.tar", last modified: Fri Jul 21 13:24:21 2023, max compression
```

## Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6.tar` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/LICENSE
--rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/__init__.py
--rw-r--r--   0        0        0    27790 2023-07-20 14:40:27.131169 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/aidraw.py
--rw-r--r--   0        0        0     6213 2023-05-30 17:03:22.535709 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
--rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
--rw-r--r--   0        0        0     3894 2023-06-12 05:12:59.000048 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
--rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
--rw-r--r--   0        0        0    16093 2023-07-16 04:28:25.749676 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/backend/base.py
--rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
--rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
--rw-r--r--   0        0        0     6015 2023-07-17 06:15:44.003068 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/backend/sd.py
--rw-r--r--   0        0        0    19419 2023-07-20 06:28:35.189871 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/config.py
--rw-r--r--   0        0        0    10771 2023-07-20 07:00:30.079891 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
--rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
--rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
--rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
--rw-r--r--   0        0        0     2754 2023-07-16 04:01:07.429355 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
--rw-r--r--   0        0        0    11332 2023-07-20 14:22:22.328291 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
--rw-r--r--   0        0        0     4139 2023-07-03 04:27:28.351334 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
--rw-r--r--   0        0        0    41887 2023-07-20 08:06:16.447962 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
--rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/extension/translation.py
--rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/fifo.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/locales/en.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/locales/jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/locales/zh.py
--rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/manage.py
--rw-r--r--   0        0        0     4670 2023-07-16 04:27:02.446129 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
--rw-r--r--   0        0        0     2111 2023-07-03 03:51:06.635888 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/utils/data.py
--rw-r--r--   0        0        0     6163 2023-07-14 13:25:19.581758 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
--rw-r--r--   0        0        0      726 2023-07-20 08:05:34.470705 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
--rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/utils/save.py
--rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/version.py
--rw-r--r--   0        0        0      730 2023-07-20 14:40:36.404645 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/pyproject.toml
--rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/LICENSE
+-rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/__init__.py
+-rw-r--r--   0        0        0    27790 2023-07-21 13:22:30.703090 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/aidraw.py
+-rw-r--r--   0        0        0     6213 2023-05-30 17:03:22.535709 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
+-rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
+-rw-r--r--   0        0        0     3894 2023-06-12 05:12:59.000048 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
+-rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
+-rw-r--r--   0        0        0    16093 2023-07-16 04:28:25.749676 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/backend/base.py
+-rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
+-rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
+-rw-r--r--   0        0        0     6015 2023-07-17 06:15:44.003068 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/backend/sd.py
+-rw-r--r--   0        0        0    18638 2023-07-21 13:24:03.431839 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/config.py
+-rw-r--r--   0        0        0    10771 2023-07-20 07:00:30.079891 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
+-rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
+-rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
+-rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
+-rw-r--r--   0        0        0     2754 2023-07-16 04:01:07.429355 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
+-rw-r--r--   0        0        0    11332 2023-07-20 14:22:22.328291 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
+-rw-r--r--   0        0        0     4139 2023-07-03 04:27:28.351334 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
+-rw-r--r--   0        0        0    41887 2023-07-20 08:06:16.447962 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
+-rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/extension/translation.py
+-rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/fifo.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/locales/en.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/locales/jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/locales/zh.py
+-rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/manage.py
+-rw-r--r--   0        0        0     4670 2023-07-16 04:27:02.446129 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
+-rw-r--r--   0        0        0     2111 2023-07-03 03:51:06.635888 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/utils/data.py
+-rw-r--r--   0        0        0     6163 2023-07-14 13:25:19.581758 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
+-rw-r--r--   0        0        0      726 2023-07-20 08:05:34.470705 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
+-rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/utils/save.py
+-rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/version.py
+-rw-r--r--   0        0        0      730 2023-07-21 13:24:21.231942 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/pyproject.toml
+-rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/PKG-INFO
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/LICENSE` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/aidraw.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/aidraw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/amusement/vits.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/amusement/vits.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/backend/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/backend/base.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/backend/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/backend/naifu.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/backend/naifu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/backend/novelai.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/backend/novelai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/backend/sd.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/backend/sd.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/config.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pathlib import Path
 import aiohttp
 import ast
 import asyncio
 import traceback
 from tqdm import tqdm
 from datetime import datetime
+import redis
 
 import aiofiles
 from nonebot import get_driver
 from nonebot.log import logger
 from pydantic import BaseSettings, validator
 from pydantic.fields import ModelField
 
@@ -121,26 +122,26 @@
     ]
     
     novelai_cndm: dict = {"controlnet_module": "canny", 
                           "controlnet_processor_res": novelai_size, 
                           "controlnet_threshold_a": 100, 
                           "controlnet_threshold_b": 250}
     
-    novelai_picaudit: int = 4  # 1为百度云图片审核, 2为本地审核功能, 请去百度云免费领取 https://ai.baidu.com/tech/imagecensoring 3为关闭, 4为使用webui，api,地址为novelai_tagger_site设置的
+    novelai_picaudit: int = 3  # 1为百度云图片审核,暂时不要使用百度云啦,要用的话使用4 , 2为本地审核功能, 请去百度云免费领取 https://ai.baidu.com/tech/imagecensoring 3为关闭, 4为使用webui，api,地址为novelai_tagger_site设置的
     novelai_pic_audit_api_key: dict = {"SECRET_KEY": "",
                                        "API_KEY": ""}  # 你的百度云API Key
     openai_api_key: str = "" # 如果要使用ChatGPTprompt生成功能, 请填写你的OpenAI API Key
     novelai_auto_icon: bool = True  # 机器人自动换头像(没写呢！)
     novelai_extra_pic_audit = True  # 是否为二次元的我, chatgpt生成tag等功能添加审核功能
     # 翻译API设置
     bing_key: str = None  # bing的翻译key
     deepl_key: str = None  # deepL的翻译key
     baidu_translate_key: dict = None  # 例:{"SECRET_KEY": "", "API_KEY": ""} # https://console.bce.baidu.com/ai/?_=1685076516634#/ai/machinetranslation/overview/index
     novelai_todaygirl = 1  # 可选值 1 和 2 两种不同的方式
-    novelai_tagger_site: str = "la.iamdiao.lol:25"  # 分析功能的地址 例如 127.0.0.1:7860
+    novelai_tagger_site: str = "la.iamdiao.lol:6884"  # 分析功能的地址 例如 127.0.0.1:7860
     vits_site: str = "la.iamdiao.lol:587"
     run_screenshot = False  # 获取服务器的屏幕截图
     is_redis_enable = True  # 是否启动redis, 启动redis以获得更多功能
     auto_match = True  # 是否自动匹配
     backend_name_list = []
     backend_site_list = []
     # 允许单群设置的设置
@@ -283,102 +284,99 @@
 try:
     import tensorflow
 except ImportError:
     logger.warning("未能成功导入tensorflow")
     logger.warning("novelai_picaudit为2时本地图片审核不可用")
 if config.is_redis_enable:
     try:
-        import redis
-    except ImportError:
-        logger.error("未找到redis库, 请先pip install redis")
-    else:
+        
         async def main():
             redis_client = []
             r1 = redis.Redis(host='localhost', port=6379, db=7)
             r2 = redis.Redis(host='localhost', port=6379, db=8)
             r3 = redis.Redis(host='localhost', port=6379, db=9)
             redis_client = [r1, r2, r3]
-            resp = r1.ping()
-            try:
-                if resp:
-                    logger.info("redis连接成功")
-                    current_date = datetime.now().date()
-                    day: str = str(int(datetime.combine(current_date, datetime.min.time()).timestamp()))
-                    if r3.exists(day):
-                        is_changed = False
-                        today_dict = r3.get(day)
-                        today_dict = ast.literal_eval(today_dict.decode('utf-8'))
-                        today_gpu_dict: dict = today_dict["gpu"]
-                        backend_name_list = list(today_gpu_dict.keys())
-                        logger.info("开始匹配redis中的后端数据")
-                        if len(backend_name_list) != len(config.backend_name_list):
-                            is_changed = True
-                        for backend_name in config.backend_name_list:
-                            if backend_name not in backend_name_list:
-                                is_changed = True
-                        if is_changed:
-                            today_gpu_dict = {}
-                            for backend_name in config.backend_name_list:
-                                today_gpu_dict[backend_name] = 0
-                            logger.info("更新redis中的后端数据...")
-                            logger.warning("请注意,本日后端的工作数量会被清零")
-                            today_dict["gpu"] = today_gpu_dict
-                            r3.set(day, str(today_dict))
-                    logger.info("开始读取webui的预设")
-                    all_style_list, all_emb_list, all_lora_list = [], [], []
-                    backend_emb, backend_lora = {}, {}
-                    all_resp_style = await this_is_a_func(0)
-                    for backend_style in all_resp_style:
-                        if backend_style is not None:
-                            for style in backend_style:
-                                all_style_list.append(json.dumps(style))
-                    logger.info("读取webui的预设完成")
-                    logger.info("开始读取webui的embs")
-                    normal_backend_index = -1
-                    all_emb_list = await this_is_a_func(1)
-                    for back_emb in all_emb_list:
-                        normal_backend_index += 1
-                        if back_emb is not None:
-                            emb_dict = {}
-                            n = 0
-                            for emb in list(back_emb["loaded"].keys()):
-                                n += 1
-                                emb_dict[n] = emb
-                            backend_emb[config.backend_name_list[normal_backend_index]] = emb_dict
-                        else:
-                            backend_emb[config.backend_name_list[normal_backend_index]] = None
-                    logger.info("开始读取webui的loras")
-                    all_lora_list = await this_is_a_func(2)
-                    normal_backend_index = -1
-                    for back_lora in all_lora_list:
-                        normal_backend_index += 1
-                        if back_lora is not None:
-                            lora_dict = {}
-                            n = 0
-                            for lora in back_lora:
-                                lora_name = lora["name"]
-                                n += 1
-                                lora_dict[n] = lora_name
-                            backend_lora[config.backend_name_list[normal_backend_index]] = lora_dict
-                        else:
-                            backend_lora[config.backend_name_list[normal_backend_index]] = None
-                    logger.info("存入数据库...")
-                    if r2.exists("emb"):
-                        r2.delete(*["style", "emb", "lora"])
-                    pipe = r2.pipeline()
-                    pipe.rpush("style", *all_style_list)
-                    pipe.set("emb", str(backend_emb))
-                    pipe.set("lora", str(backend_lora))
-                    pipe.execute()
+            logger.info("redis连接成功")
+            current_date = datetime.now().date()
+            day: str = str(int(datetime.combine(current_date, datetime.min.time()).timestamp()))
+            
+            if r3.exists(day):
+                is_changed = False
+                today_dict = r3.get(day)
+                today_dict = ast.literal_eval(today_dict.decode('utf-8'))
+                today_gpu_dict: dict = today_dict["gpu"]
+                backend_name_list = list(today_gpu_dict.keys())
+                logger.info("开始匹配redis中的后端数据")
+                if len(backend_name_list) != len(config.backend_name_list):
+                    is_changed = True
+                for backend_name in config.backend_name_list:
+                    if backend_name not in backend_name_list:
+                        is_changed = True
+                if is_changed:
+                    today_gpu_dict = {}
+                    for backend_name in config.backend_name_list:
+                        today_gpu_dict[backend_name] = 0
+                    logger.info("更新redis中的后端数据...")
+                    logger.warning("请注意,本日后端的工作数量会被清零")
+                    today_dict["gpu"] = today_gpu_dict
+                    r3.set(day, str(today_dict))
+            logger.info("开始读取webui的预设")
+            all_style_list, all_emb_list, all_lora_list = [], [], []
+            backend_emb, backend_lora = {}, {}
+            all_resp_style = await this_is_a_func(0)
+            
+            for backend_style in all_resp_style:
+                if backend_style is not None:
+                    for style in backend_style:
+                        all_style_list.append(json.dumps(style))
+            logger.info("读取webui的预设完成")
+            logger.info("开始读取webui的embs")
+            normal_backend_index = -1
+            all_emb_list = await this_is_a_func(1)
+            
+            for back_emb in all_emb_list:
+                normal_backend_index += 1
+                if back_emb is not None:
+                    emb_dict = {}
+                    n = 0
+                    for emb in list(back_emb["loaded"].keys()):
+                        n += 1
+                        emb_dict[n] = emb
+                    backend_emb[config.backend_name_list[normal_backend_index]] = emb_dict
+                else:
+                    backend_emb[config.backend_name_list[normal_backend_index]] = None
+            logger.info("开始读取webui的loras")
+            all_lora_list = await this_is_a_func(2)
+            normal_backend_index = -1
+            
+            for back_lora in all_lora_list:
+                normal_backend_index += 1
+                if back_lora is not None:
+                    lora_dict = {}
+                    n = 0
+                    for lora in back_lora:
+                        lora_name = lora["name"]
+                        n += 1
+                        lora_dict[n] = lora_name
+                    backend_lora[config.backend_name_list[normal_backend_index]] = lora_dict
                 else:
-                    logger.error("redis连接失败")
-                    redis_client = None
-            except Exception:
-                logger.error(traceback.print_exc())
-                logger.error("出现了意外错误, 已经暂停redis使用")
-                redis_client = None
+                    backend_lora[config.backend_name_list[normal_backend_index]] = None
+            logger.info("存入数据库...")
+            
+            if r2.exists("emb"):
+                r2.delete(*["style", "emb", "lora"])
+            pipe = r2.pipeline()
+            pipe.rpush("style", *all_style_list)
+            pipe.set("emb", str(backend_emb))
+            pipe.set("lora", str(backend_lora))
+            pipe.execute()
+            
             return redis_client
+        
         redis_client = asyncio.run(main())
+    except Exception:
+        redis_client = None
+        logger.warning("redis初始化失败, 已经禁用redis")
 
 logger.info(f"加载config完成" + str(config))
 logger.info(f"后端数据加载完成, 共有{len(config.backend_name_list)}个后端被加载")
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/extension/anlas.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/extension/anlas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/extension/control_net.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/extension/control_net.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/extension/translation.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/extension/translation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/manage.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/utils/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/utils/data.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/utils/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/utils/save.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/utils/save.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/nonebot_plugin_stable_diffusion_diao/version.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/nonebot_plugin_stable_diffusion_diao/version.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.5.6/pyproject.toml` & `nonebot_plugin_stable_diffusion_diao-0.3.9.5.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-stable-diffusion-diao"
-version = "0.3.9.5.6"
+version = "0.3.9.5.7"
 description = "主要面对stable-diffusion-webui-api的nonebot2插件"
 authors = [
     { name = "DiaoDaiaChan", email = "diaodaiachan@qq.com" },
 ]
 dependencies = [
     "aiofiles>=23.1.0",
     "aiohttp>=3.8.4",
```

