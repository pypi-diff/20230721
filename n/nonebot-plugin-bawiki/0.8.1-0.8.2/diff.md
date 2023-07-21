# Comparing `tmp/nonebot_plugin_bawiki-0.8.1.tar.gz` & `tmp/nonebot_plugin_bawiki-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bawiki-0.8.1.tar", last modified: Sun Jun 25 16:16:03 2023, max compression
+gzip compressed data, was "nonebot_plugin_bawiki-0.8.2.tar", last modified: Fri Jul 21 07:53:24 2023, max compression
```

## Comparing `nonebot_plugin_bawiki-0.8.1.tar` & `nonebot_plugin_bawiki-0.8.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1068 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/LICENSE
--rw-r--r--   0        0        0     9414 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/README.md
--rw-r--r--   0        0        0      734 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/__init__.py
--rw-r--r--   0        0        0      947 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/__init__.py
--rw-r--r--   0        0        0     3827 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/arona.py
--rw-r--r--   0        0        0     2320 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/calender.py
--rw-r--r--   0        0        0     1265 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/clear_cache.py
--rw-r--r--   0        0        0     1218 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/craft.py
--rw-r--r--   0        0        0     1003 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/emoji.py
--rw-r--r--   0        0        0     2580 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/event.py
--rw-r--r--   0        0        0      976 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/furniture.py
--rw-r--r--   0        0        0     6327 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/gacha.py
--rw-r--r--   0        0        0     3555 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/global_future.py
--rw-r--r--   0        0        0     1775 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/level_guide.py
--rw-r--r--   0        0        0     1428 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/manga.py
--rw-r--r--   0        0        0     4356 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/raid.py
--rw-r--r--   0        0        0     3597 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/stu_fav.py
--rw-r--r--   0        0        0     1868 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/stu_rank.py
--rw-r--r--   0        0        0     1625 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/stu_wiki_gamekee.py
--rw-r--r--   0        0        0     2011 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/stu_wiki_schale.py
--rw-r--r--   0        0        0     3375 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/time_atk.py
--rw-r--r--   0        0        0     3255 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/voice.py
--rw-r--r--   0        0        0     1152 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/config.py
--rw-r--r--   0        0        0        0 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/data/__init__.py
--rw-r--r--   0        0        0     1541 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/data/arona.py
--rw-r--r--   0        0        0     5814 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/data/bawiki.py
--rw-r--r--   0        0        0     9814 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/data/gamekee.py
--rw-r--r--   0        0        0    18830 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/data/schaledb.py
--rw-r--r--   0        0        0     7390 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/gacha.py
--rw-r--r--   0        0        0     1358 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/help/__init__.py
--rw-r--r--   0        0        0     1784 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/help/manual.py
--rw-r--r--   0        0        0     2216 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/help/pic_menu.py
--rw-r--r--   0        0        0      919 2023-06-25 16:15:31.670212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/__init__.py
--rw-r--r--   0        0        0    21514 2023-06-25 16:15:31.674212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/calender_banner.png
--rw-r--r--   0        0        0  1685142 2023-06-25 16:15:31.674212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_bg.png
--rw-r--r--   0        0        0    13956 2023-06-25 16:15:31.674212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png
--rw-r--r--   0        0        0     2408 2023-06-25 16:15:31.674212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png
--rw-r--r--   0        0        0     4391 2023-06-25 16:15:31.674212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_new.png
--rw-r--r--   0        0        0    10375 2023-06-25 16:15:31.674212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_pickup.png
--rw-r--r--   0        0        0     2022 2023-06-25 16:15:31.674212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_star.png
--rw-r--r--   0        0        0    14652 2023-06-25 16:15:31.674212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png
--rw-r--r--   0        0        0  1764190 2023-06-25 16:15:31.678212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gradient.png
--rw-r--r--   0        0        0     4596 2023-06-25 16:15:31.678212 nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/util.py
--rw-r--r--   0        0        0     1481 2023-06-25 16:16:03.258182 nonebot_plugin_bawiki-0.8.1/pyproject.toml
--rw-r--r--   0        0        0    10865 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-21 07:52:55.471583 nonebot_plugin_bawiki-0.8.2/LICENSE
+-rw-r--r--   0        0        0     9655 2023-07-21 07:52:55.471583 nonebot_plugin_bawiki-0.8.2/README.md
+-rw-r--r--   0        0        0      734 2023-07-21 07:52:55.471583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/__init__.py
+-rw-r--r--   0        0        0      947 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/__init__.py
+-rw-r--r--   0        0        0     3758 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/arona.py
+-rw-r--r--   0        0        0     2330 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/calender.py
+-rw-r--r--   0        0        0     1265 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/clear_cache.py
+-rw-r--r--   0        0        0     1228 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/craft.py
+-rw-r--r--   0        0        0     1013 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/emoji.py
+-rw-r--r--   0        0        0     2600 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/event.py
+-rw-r--r--   0        0        0      986 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/furniture.py
+-rw-r--r--   0        0        0     6372 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/gacha.py
+-rw-r--r--   0        0        0     3555 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/global_future.py
+-rw-r--r--   0        0        0     1795 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/level_guide.py
+-rw-r--r--   0        0        0     1438 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/manga.py
+-rw-r--r--   0        0        0     4376 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/raid.py
+-rw-r--r--   0        0        0     3617 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/stu_fav.py
+-rw-r--r--   0        0        0     1878 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/stu_rank.py
+-rw-r--r--   0        0        0     1635 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/stu_wiki_gamekee.py
+-rw-r--r--   0        0        0     2031 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/stu_wiki_schale.py
+-rw-r--r--   0        0        0     3395 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/time_atk.py
+-rw-r--r--   0        0        0     4201 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/voice.py
+-rw-r--r--   0        0        0     1152 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/config.py
+-rw-r--r--   0        0        0        0 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/__init__.py
+-rw-r--r--   0        0        0     1541 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/arona.py
+-rw-r--r--   0        0        0     5814 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/bawiki.py
+-rw-r--r--   0        0        0     7398 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/gacha.py
+-rw-r--r--   0        0        0    11340 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/gamekee.py
+-rw-r--r--   0        0        0    18840 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/schaledb.py
+-rw-r--r--   0        0        0     1358 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/help/__init__.py
+-rw-r--r--   0        0        0     1784 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/help/manual.py
+-rw-r--r--   0        0        0     2226 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/help/pic_menu.py
+-rw-r--r--   0        0        0      919 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/__init__.py
+-rw-r--r--   0        0        0    21514 2023-07-21 07:52:55.475583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/calender_banner.png
+-rw-r--r--   0        0        0  1685142 2023-07-21 07:52:55.479583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_bg.png
+-rw-r--r--   0        0        0    13956 2023-07-21 07:52:55.479583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png
+-rw-r--r--   0        0        0     2408 2023-07-21 07:52:55.479583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png
+-rw-r--r--   0        0        0     4391 2023-07-21 07:52:55.479583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_new.png
+-rw-r--r--   0        0        0    10375 2023-07-21 07:52:55.479583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_pickup.png
+-rw-r--r--   0        0        0     2022 2023-07-21 07:52:55.479583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_star.png
+-rw-r--r--   0        0        0    14652 2023-07-21 07:52:55.479583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png
+-rw-r--r--   0        0        0  1764190 2023-07-21 07:52:55.483583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gradient.png
+-rw-r--r--   0        0        0     4668 2023-07-21 07:52:55.483583 nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/util.py
+-rw-r--r--   0        0        0     1481 2023-07-21 07:53:24.712021 nonebot_plugin_bawiki-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0    11106 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.8.2/PKG-INFO
```

### Comparing `nonebot_plugin_bawiki-0.8.1/LICENSE` & `nonebot_plugin_bawiki-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.1/README.md` & `nonebot_plugin_bawiki-0.8.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -171,14 +171,19 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.8.2
+
+- 修改了 `ba语音` 指令的特性，兼容了有中配语音的学生，请查看该指令帮助获取详细信息
+- 删除了 `arona` 指令模糊搜索展示类别的功能，因为模糊搜索时 `type` 固定为 `0` 了
+
 ### 0.8.1
 
 - 使用 `arona` 指令模糊搜索的时候会显示图片类别了
 
 ### 0.8.0
 
 - 整理项目结构
```

#### html2text {}

```diff
@@ -52,17 +52,22 @@
 (https://lonqie.github.io/SchaleDB/) & [Arona Bot](https://
 doc.arona.diyigemt.com/api/) - æä»¶æ°æ®æºæä¾  ### `bawiki-data`
 æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/bawiki-
 data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
 å®å¨ææ¿ä¸å°½â¦â¦ - [ç±åçµ](https://afdian.net/@lgc2333) -
 èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ ![è®¨é¥­](https://raw.githubusercontent.com/
 lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ###
-0.8.1 - ä½¿ç¨ `arona` æä»¤æ¨¡ç³æç´¢çæ¶åä¼æ¾ç¤ºå¾çç±»å«äº ###
-0.8.0 - æ´çé¡¹ç®ç»æ - æ·»å åç½®å¸®å©æä»¤ `baå¸®å©` - æ·»å  Arona
-Bot æ°æ®æºæä»¤ `arona` - æ·»å äºéç½®é¡¹
+0.8.2 - ä¿®æ¹äº `baè¯­é³`
+æä»¤çç¹æ§ï¼å¼å®¹äºæä¸­éè¯­é³çå­¦çï¼è¯·æ¥çè¯¥æä»¤å¸®å©è·åè¯¦ç»ä¿¡æ¯
+- å é¤äº `arona`
+æä»¤æ¨¡ç³æç´¢å±ç¤ºç±»å«çåè½ï¼å ä¸ºæ¨¡ç³æç´¢æ¶ `type`
+åºå®ä¸º `0` äº ### 0.8.1 - ä½¿ç¨ `arona`
+æä»¤æ¨¡ç³æç´¢çæ¶åä¼æ¾ç¤ºå¾çç±»å«äº ### 0.8.0 -
+æ´çé¡¹ç®ç»æ - æ·»å åç½®å¸®å©æä»¤ `baå¸®å©` - æ·»å  Arona Bot
+æ°æ®æºæä»¤ `arona` - æ·»å äºéç½®é¡¹
 `BA_ARONA_API_URL`ã`BA_ARONA_CDN_URL`ã`BA_CLEAR_REQ_CACHE_INTERVAL`ã`BA_AUTO_CLEAR_ARONA_CACHE`
 - å¶ä»å°æ´æ¹ï¼æ´æ¢ `aiohttp` ä¸º `httpx` ç­ï¼ ### 0.7.10 -
 æ·»å æä»¤ `baå³å¡` ### 0.7.9 - æ·»å éç½®é¡¹ `BA_VOICE_USE_CARD` ###
 0.7.8 - ð NoneBot 2.0 ð ### 0.7.7 - ä¿®å¤ bug ### 0.7.6 -
 ä¿®å¤å¡æ± ä¸ºç©ºä¸ä¼æç¤ºç bug ### 0.7.5 -
 æä»¶å¯ä»¥èªå¨å¸®ä½ éç½® PicMenu çå­ä½äº - ç»æ½å¡æ°å¢äºå·å´
 ### 0.7.2 ~ 0.7.4 - ä¿®å¤ bug ### 0.7.1 - æ´æ¹éç½®é¡¹åç§° ### 0.7.0 -
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/__init__.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 require("nonebot_plugin_apscheduler")
 require("nonebot_plugin_htmlrender")
 
 from .command import load_commands  # noqa: E402
 from .config import Cfg as Cfg  # noqa: E402
 from .help import extra, register_help_cmd, usage  # noqa: E402
 
-__version__ = "0.8.1"
+__version__ = "0.8.2"
 __plugin_meta__ = PluginMetadata(
     name="BAWiki",
     description="碧蓝档案Wiki插件",
     usage=usage,
     homepage="https://github.com/lgc-NB2Dev/nonebot-plugin-bawiki",
     type="application",
     config=Cfg,
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/__init__.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/arona.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/arona.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,18 +74,15 @@
     if not res:
         await matcher.finish("没有找到相关图片")
 
     if len(res) == 1:
         await send_image(matcher, res[0])
 
     state["res"] = res
-    list_txt = "\n".join(
-        f"{i}. {r.name} ({IMAGE_TYPE_MAP.get(r.type, '未知分类')})"
-        for i, r in enumerate(res, 1)
-    )
+    list_txt = "\n".join(f"{i}. {r.name}" for i, r in enumerate(res, 1))
     await matcher.pause(
         f"Arona 查到了多个结果，请 sensei 发送序号选择~\n{list_txt}\nTip：发送 0 取消选择",
     )
 
 
 @cmd_arona.handle()
 async def _(event: MessageEvent, matcher: Matcher, state: T_State):
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/calender.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/calender.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,10 +60,10 @@
                 ],
             )
             await matcher.finish()
         else:
             await matcher.finish(await game_kee_calender())
     except (FinishedException, ActionFailed):  # type: ignore
         raise
-    except:
+    except Exception:
         logger.exception("绘制日程表图片出错")
         await matcher.finish("绘制日程表图片出错，请检查后台输出")
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/clear_cache.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/clear_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/craft.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/craft.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,12 +32,12 @@
 cmd_craft_wiki = on_command("ba制造", aliases={"ba合成", "ba制作"})
 
 
 @cmd_craft_wiki.handle()
 async def _(matcher: Matcher):
     try:
         im = await db_wiki_craft()
-    except:
+    except Exception:
         logger.exception("获取合成wiki图片错误")
         await matcher.finish("获取图片失败，请检查后台输出")
 
     await matcher.finish(Message(im))
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/emoji.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/emoji.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,11 +26,11 @@
 
 
 @cmd_random_emoji.handle()
 async def _(matcher: Matcher):
     try:
         emojis = await db_get_emoji()
         emo = await db_get(random.choice(emojis), True)
-    except:
+    except Exception:
         logger.exception("获取表情失败")
         await matcher.finish("获取表情失败，请检查后台输出")
     await matcher.finish(MessageSegment.image(emo))
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/event.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/event.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,24 +54,24 @@
     if server:
         try:
             common = await schale_get_common()
             for s in server:
                 ev = common["regions"][s]["current_events"]
                 if e := find_current_event(ev):
                     events.append((e[0]["event"]) % 10000)
-        except:
+        except Exception:
             logger.exception("获取当前活动失败")
             await matcher.finish("获取当前活动失败")
 
         if not events:
             await matcher.finish("当前服务器没有正在进行的活动")
 
     else:
         events.append(recover_alia(arg, await db_get_event_alias()))
 
     try:
         ret = await asyncio.gather(*[db_wiki_event(x) for x in events])
-    except:
+    except Exception:
         logger.exception("获取活动wiki出错")
         await matcher.finish("获取图片出错，请检查后台输出")
 
     await matcher.finish(splice_msg(ret))
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/furniture.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/furniture.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,12 +24,12 @@
 cmd_furniture_wiki = on_command("ba互动家具")
 
 
 @cmd_furniture_wiki.handle()
 async def _(matcher: Matcher):
     try:
         im = await db_wiki_furniture()
-    except:
+    except Exception:
         logger.exception("获取互动家具wiki图片错误")
         await matcher.finish("获取图片失败，请检查后台输出")
 
     await matcher.finish(Message(im))
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/gacha.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/gacha.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     MessageSegment,
 )
 from nonebot.internal.matcher import Matcher
 from nonebot.log import logger
 from nonebot.params import CommandArg
 
 from ..data.bawiki import db_get_gacha_data, db_get_stu_alias
+from ..data.gacha import gacha, get_gacha_cool_down, set_gacha_cool_down
 from ..data.schaledb import schale_get_stu_dict
-from ..gacha import gacha, get_gacha_cool_down, set_gacha_cool_down
 from ..util import recover_alia
 
 if TYPE_CHECKING:
     from . import HelpList
 
 help_list: "HelpList" = [
     {
@@ -92,15 +92,15 @@
         if "常驻" in arg:
             current = GachaPool(name="常驻池", pool=[])
         else:
             pool = []
             try:
                 stu_li = await schale_get_stu_dict()
                 stu_alias = await db_get_stu_alias()
-            except:
+            except Exception:
                 logger.exception("获取学生列表或别名失败")
                 await matcher.finish("获取学生列表或别名失败，请检查后台输出")
 
             for i in arg.split():
                 if not (stu := stu_li.get(recover_alia(i, stu_alias))):
                     await matcher.finish(f"未找到学生 {i}")
                 if stu["StarGrade"] == 1:
@@ -111,15 +111,15 @@
                 name=f"自定义卡池（{'、'.join([x['Name'] for x in pool])}）",
                 pool=[x["Id"] for x in pool],
             )
 
     else:
         try:
             gacha_data = await db_get_gacha_data()
-        except:
+        except Exception:
             logger.exception("获取抽卡基本数据失败")
             await matcher.finish("获取抽卡基本数据失败，请检查后台输出")
 
         pool_data = gacha_data["current_pools"]
         first_pool = get_1st_pool(gacha_data)
         if not first_pool:
             await matcher.finish("当前没有可切换的卡池")
@@ -156,15 +156,15 @@
 
     gacha_times = 10
     if arg and ((not arg.isdigit()) or (not (1 <= (gacha_times := int(arg)) <= 90))):
         await matcher.finish("请输入有效的抽卡次数，在1~90之间")
 
     try:
         gacha_data = await db_get_gacha_data()
-    except:
+    except Exception:
         logger.exception("获取抽卡基本数据失败")
         await matcher.finish("获取抽卡基本数据失败，请检查后台输出")
 
     pool_obj = gacha_pool_index.get(qq := event.get_user_id()) or get_1st_pool(
         gacha_data,
     )
     if not pool_obj:
@@ -178,12 +178,12 @@
                     qq,
                     10 if gacha_times >= 10 else gacha_times,
                     gacha_data,
                     pool_obj.pool,
                 ),
             )
             gacha_times -= 10
-    except:
+    except Exception:
         logger.exception("抽卡错误")
         await matcher.finish("抽卡出错了，请检查后台输出")
 
     await matcher.finish(MessageSegment.at(qq) + f"当前抽取卡池：{pool_obj.name}" + img)
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/global_future.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/global_future.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/level_guide.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/level_guide.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,25 +36,25 @@
 async def _(matcher: Matcher, arg: Message = CommandArg()):
     arg_str = arg.extract_plain_text().strip().upper()
     if not arg_str:
         await matcher.finish("请输入关卡名称")
 
     try:
         levels = await get_level_list()
-    except:
+    except Exception:
         logger.exception("获取关卡列表失败")
         await matcher.finish("获取关卡列表失败，请检查后台输出")
 
     if arg_str not in levels:
         await matcher.finish("未找到该关卡，请检查关卡名称是否正确")
 
     cid = levels[arg_str]
     try:
         imgs = await extract_content_pic(cid)
-    except:
+    except Exception:
         logger.exception("获取攻略图片失败")
         await matcher.finish("获取攻略图片失败，请检查后台输出")
 
     msg = Message()
     msg += f"https://ba.gamekee.com/{cid}.html\n"
     msg += [MessageSegment.image(x) for x in imgs]
     await matcher.finish(msg)
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/manga.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/manga.py`

 * *Files 17% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         if url.endswith(".webp"):
             p = BuildImage.open(BytesIO(p)).save_png()
         return p
 
     try:
         manga: MangaDict = random.choice(await db_get_manga())
         pics = await asyncio.gather(*[get_pic(x) for x in manga["pics"]])
-    except:
+    except Exception:
         logger.exception("获取漫画失败")
         await matcher.finish("获取漫画失败，请检查后台输出")
 
     await matcher.finish(
         Message()
         + f'{manga["title"]}\n-=-=-=-=-=-=-=-\n{manga["detail"]}'
         + [MessageSegment.image(x) for x in pics],
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/raid.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/raid.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             common = await schale_get_common()
             for s in server:
                 raid = common["regions"][s]["current_raid"]
                 if (r := find_current_event(raid)) and (raid := r[0]["raid"]) < 1000:
                     tasks.append(
                         db_wiki_raid(raid, [s], args.wiki, r[0].get("terrain")),
                     )
-        except:
+        except Exception:
             logger.exception("获取当前总力战失败")
             await matcher.finish("获取当前总力战失败")
 
         if not tasks:
             await matcher.finish("目前服务器没有正在进行的总力战，请手动指定")
     else:
         tasks.append(
@@ -115,12 +115,12 @@
                     else None
                 ),
             ),
         )
 
     try:
         ret = await asyncio.gather(*tasks)
-    except:
+    except Exception:
         logger.exception("获取总力战wiki失败")
         await matcher.finish("获取图片失败，请检查后台输出")
 
     await matcher.finish(splice_msg(ret))
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/stu_fav.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/stu_fav.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,26 +64,26 @@
         if arg > 9:
             await matcher.finish("学生解锁L2D最高只需要羁绊等级9")
         if arg < 1:
             await matcher.finish("学生解锁L2D最低只需要羁绊等级1")
 
         try:
             p = await draw_fav_li(arg)
-        except:
+        except Exception:
             logger.exception("绘制图片出错")
             await matcher.finish("绘制图片出错，请检查后台输出")
 
         await matcher.finish(p)
 
     # 学生名称
     arg = await recover_stu_alia(arg)
 
     try:
         ret = await schale_get_stu_dict()
-    except:
+    except Exception:
         logger.exception("获取学生列表出错")
         await matcher.finish("获取学生列表表出错，请检查后台输出")
 
     if stu := ret.get(arg):
         if not (lvl := stu["MemoryLobby"]):
             await matcher.finish("该学生没有L2D")
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/stu_rank.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/stu_rank.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,12 +49,12 @@
     if arg == "总览" or arg == "全部" or arg.lower() == "all":
         arg = "all"
     else:
         arg = await recover_stu_alia(arg)
 
     try:
         im = await db_wiki_stu(arg)
-    except:
+    except Exception:
         logger.exception("获取角评出错")
         await matcher.finish("获取角评出错，请检查后台输出")
 
     await matcher.finish(im)
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/stu_wiki_gamekee.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/stu_wiki_gamekee.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 async def _(matcher: Matcher, cmd_arg: Message = CommandArg()):
     arg = cmd_arg.extract_plain_text().strip()
     if not arg:
         await matcher.finish("请提供学生名称")
 
     try:
         ret = await game_kee_get_stu_cid_li()
-    except:
+    except Exception:
         logger.exception("获取学生列表出错")
         await matcher.finish("获取学生列表出错，请检查后台输出")
 
     if not ret:
         await matcher.finish("没有获取到学生列表数据")
 
     if not (sid := ret.get(await recover_stu_alia(arg, True))):
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/stu_wiki_schale.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/stu_wiki_schale.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,27 +37,27 @@
 async def _(matcher: Matcher, cmd_arg: Message = CommandArg()):
     arg = cmd_arg.extract_plain_text().strip()
     if not arg:
         await matcher.finish("请提供学生名称")
 
     try:
         ret = await schale_get_stu_dict()
-    except:
+    except Exception:
         logger.exception("获取学生列表出错")
         await matcher.finish("获取学生列表表出错，请检查后台输出")
 
     if not ret:
         await matcher.finish("没有获取到学生列表数据")
 
     if not (data := ret.get(await recover_stu_alia(arg))):
         await matcher.finish("未找到该学生")
 
     stu_name = data["PathName"]
     await matcher.send(f"请稍等，正在截取SchaleDB页面～\n{config.ba_schale_url}?chara={stu_name}")
 
     try:
         img = MessageSegment.image(await schale_get_stu_info(stu_name))
-    except:
+    except Exception:
         logger.exception(f"截取schale db页面出错 chara={stu_name}")
         await matcher.finish("截取页面出错，请检查后台输出")
 
     await matcher.finish(img)
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/time_atk.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/time_atk.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,26 +62,26 @@
     if server:
         try:
             common = await schale_get_common()
             for s in server:
                 raid = common["regions"][s]["current_raid"]
                 if (r := find_current_event(raid)) and (raid := r[0]["raid"]) >= 1000:
                     events.append(raid)
-        except:
+        except Exception:
             logger.exception("获取当前综合战术考试失败")
             await matcher.finish("获取当前综合战术考试失败")
 
         if not events:
             await matcher.finish("当前服务器没有正在进行的综合战术考试")
 
     else:
         if (not str(arg).isdigit()) or ((arg := int(arg)) < 1):
             await matcher.finish("综合战术考试ID需为整数，从1开始，代表第1个综合战术考试")
         events.append(arg)
 
     try:
         ret = await asyncio.gather(*[db_wiki_time_atk(x) for x in events])
-    except:
+    except Exception:
         logger.exception("获取综合战术考试wiki出错")
         await matcher.finish("获取图片出错，请检查后台输出")
 
     await matcher.finish(splice_msg(ret))
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/command/voice.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/command/voice.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,85 +19,108 @@
     {
         "func": "学生语音",
         "trigger_method": "指令",
         "trigger_condition": "ba语音",
         "brief_des": "发送学生语音",
         "detail_des": (
             "从GameKee爬取学生语音并发送\n"
-            "指定关键词时会从匹配结果中随机选择一个语音发送\n"
+            "可以用 语音名称 或 中文或日文台词 搜索角色语音\n"
+            "如果有多个结果，则会从中随机选择一个语音发送\n"
             " \n"
-            "可以用这些指令触发：\n"
-            "- <ft color=(238,120,0)>ba语音</ft>\n"
+            "默认获取日配语音，如果角色有中配，则可以在指令后方带上 `中配` 来获取\n"
+            "如果找不到中配语音对应的台词，则会展示日配台词\n"
+            # " \n"
+            # "可以用这些指令触发：\n"
+            # "- <ft color=(238,120,0)>ba语音</ft>\n"
             " \n"
             "指令示例：\n"
             "- <ft color=(238,120,0)>ba语音 忧</ft>\n"
-            "- <ft color=(238,120,0)>ba语音 美游 被cc</ft>"
+            "- <ft color=(238,120,0)>ba语音 美游 被cc</ft>\n"
+            "- <ft color=(238,120,0)>ba语音 水大叔 好热</ft>\n"
+            "- <ft color=(238,120,0)>ba语音中配 白子</ft>\n"
+            "- <ft color=(238,120,0)>ba语音中配 大叔 睡午觉</ft>"
         ),
     },
 ]
 
 
 cmd_voice = on_command("ba语音")
 
 
 @cmd_voice.handle()
 async def _(matcher: Matcher, cmd_arg: Message = CommandArg()):
     arg = cmd_arg.extract_plain_text().strip()
+    is_chinese = False
+    if arg.startswith("中配"):
+        arg = arg[2:].strip()
+        is_chinese = True
+
     if not arg:
         await matcher.finish("请提供学生名称")
 
     arg = arg.split()
     arg_len = len(arg)
     name = " ".join(arg[:-1]) if arg_len > 1 else arg[0]
     v_type = arg[-1].strip().lower() if arg_len > 1 else None
 
     try:
         ret = await game_kee_get_stu_li()
-    except:
+    except Exception:
         logger.exception("获取学生列表出错")
         await matcher.finish("获取学生列表出错，请检查后台输出")
 
     if not ret:
         await matcher.finish("没有获取到学生列表数据")
 
     try:
         org_stu_name = await recover_stu_alia(name, True)
         stu_name = await schale_to_gamekee(org_stu_name)
-    except:
+    except Exception:
         logger.exception("还原学生别名失败")
         await matcher.finish("还原学生别名失败，请检查后台输出")
 
     if not (stu_info := ret.get(stu_name)):
         await matcher.finish("未找到该学生")
 
-    voices = await game_kee_get_voice(stu_info["content_id"])
+    voices = await game_kee_get_voice(stu_info["content_id"], is_chinese)
     if v_type:
-        voices = [x for x in voices if v_type in x.title.lower()]
+        voices = [
+            x
+            for x in voices
+            if (
+                (v_type in x.title.lower())
+                or (v_type in x.jp.lower())
+                or (v_type in x.cn.lower())
+            )
+        ]
     if not voices:
         await matcher.finish("没找到符合要求的语音捏")
 
     v: GameKeeVoice = random.choice(voices)
-
-    im = [f"学生 {org_stu_name} 语音 {v.title}\n-=-=-=-=-=-=-=-"]
-    if v.jp:
-        im.append(v.jp)
-    if v.cn:
-        im.append(v.cn)
+    voice_type = "中配" if is_chinese else "日配"
+    im = [f"学生 {org_stu_name} {voice_type}语音 {v.title}"]
+    if v.jp or v.cn:
+        im.append("-=-=-=-=-=-=-=-")
+        if v.jp:
+            im.append(v.jp)
+        if v.cn:
+            im.append(v.cn)
     await matcher.send("\n".join(im))
+
     if config.ba_voice_use_card:
-        await matcher.send(
+        await matcher.finish(
             MessageSegment(
                 "music",
                 {
                     "type": "custom",
                     "subtype": "163",
                     "url": v.url,
                     "voice": v.url,
                     "title": v.title,
                     "content": org_stu_name,
                     "image": f'http:{stu_info["icon"]}',
                 },
             ),
         )
-    else:
-        v_data = await async_req(v.url, raw=True)
-        await matcher.send(MessageSegment.record(v_data))
+
+    v_data = await async_req(v.url, raw=True)
+    await matcher.finish(MessageSegment.record(v_data))
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/config.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/data/arona.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/arona.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/data/bawiki.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/bawiki.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/data/gamekee.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/gamekee.py`

 * *Files 17% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
 async def send_wiki_page(sid: int, matcher: Matcher) -> NoReturn:
     url = game_kee_page_url(sid)
     await matcher.send(f"请稍等，正在截取Wiki页面……\n{url}")
 
     try:
         img = await game_kee_get_page(url)
-    except:
+    except Exception:
         logger.exception(f"截取wiki页面出错 {url}")
         await matcher.finish("截取页面出错，请检查后台输出")
 
     await matcher.finish(MessageSegment.image(img))
 
 
 async def game_kee_calender() -> Union[MessageSegment, str]:
@@ -132,15 +132,15 @@
         if has_pic and (_p := it.get("picture")):
             try:
                 _p = (
                     BuildImage.open(BytesIO(await async_req(f"https:{_p}", raw=True)))
                     .resize_width(1290)
                     .circle_corner(15)
                 )
-            except:
+            except Exception:
                 logger.exception("下载日程表图片失败")
 
         begin = datetime.fromtimestamp(it["begin_at"])
         end = datetime.fromtimestamp(it["end_at"])
         started = begin <= now
         time_remain = (end if started else begin) - now
         dd, hh, mm, ss = parse_time_delta(time_remain)
@@ -267,40 +267,89 @@
 class GameKeeVoice:
     title: str
     jp: str
     cn: str
     url: str
 
 
-async def game_kee_get_voice(cid) -> List[GameKeeVoice]:
+def parse_voice_elem(elem: Tag) -> GameKeeVoice:
+    url: str = cast(str, elem["src"])
+    if not url.startswith("http"):
+        url = f"https:{url}"
+
+    tr1: Tag = elem.parent.parent.parent.parent  # type: ignore
+    tds: ResultSet[Tag] = tr1.find_all("td")
+    title = tds[0].text.strip()
+    jp = "\n".join(tds[2].stripped_strings)
+
+    tr2 = tr1.next_sibling
+    cn = "\n".join(tr2.stripped_strings)  # type: ignore
+    return GameKeeVoice(title, jp, cn, url)
+
+
+def merge_voice_dialogue(voices: List[List[GameKeeVoice]]) -> List[List[GameKeeVoice]]:
+    main_voices = voices[0]
+    other_voice_entries = voices[1:]
+
+    for voice_entry in other_voice_entries:
+        for voice in (x for x in voice_entry if (not x.jp) or (not x.cn)):
+            corresponding_voice = next(
+                (x for x in main_voices if x.title == voice.title),
+                None,
+            )
+            if not corresponding_voice:
+                continue
+
+            if not voice.jp:
+                voice.jp = corresponding_voice.jp
+            if not voice.cn:
+                voice.cn = corresponding_voice.cn
+
+    return voices
+
+
+async def game_kee_get_voice(cid: int, is_chinese: bool = False) -> List[GameKeeVoice]:
     wiki_html = (
         cast(
             dict,
             await game_kee_request(f"v1/content/detail/{cid}"),
         )
     )["content"]
     bs = BeautifulSoup(wiki_html, "lxml")
-    audios = bs.select(".mould-table>tbody>tr>td>div>div>audio")
-
-    parsed: List[GameKeeVoice] = []
-    for au in audios:
-        url: str = cast(str, au["src"])
-        if not url.startswith("http"):
-            url = f"https:{url}"
-
-        tr1: Tag = au.parent.parent.parent.parent  # type: ignore
-        tds: ResultSet[Tag] = tr1.find_all("td")
-        title = tds[0].text.strip()
-        jp = "\n".join(tds[2].stripped_strings)
-
-        tr2 = tr1.next_sibling
-        cn = "\n".join(tr2.stripped_strings)  # type: ignore
-        parsed.append(GameKeeVoice(title, jp, cn, url))
 
-    return parsed
+    multi_lang_voices = [
+        [parse_voice_elem(x) for x in audios]
+        for table_fathers in bs.select(".slide-item")
+        if (
+            # 选择 tables
+            (tables := table_fathers.select(".table-overflow > .mould-table"))
+            # 检查 tables 中是否有语音，如果有，就取出语音到变量 aus -> audios
+            and (
+                audios := next(
+                    (aus for child in tables if (aus := child.find_all("audio"))),
+                    None,
+                )
+            )
+        )
+    ]
+    if multi_lang_voices:
+        return merge_voice_dialogue(multi_lang_voices)[1 if is_chinese else 0]
+
+    # 没有中配
+    if is_chinese:
+        return []
+    return list(
+        itertools.chain(
+            *(
+                [parse_voice_elem(x) for x in a]
+                for x in bs.select(".mould-table")
+                if (a := x.find_all("audio"))
+            )
+        )
+    )
 
 
 async def get_level_list() -> Dict[str, int]:
     entry = cast(dict, await game_kee_request("v1/wiki/entry"))
     entry_list: List[Dict] = entry["entry_list"]
     guide_entry: List[Dict] = next(x["child"] for x in entry_list if x["id"] == 50284)
     levels = itertools.chain(
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/data/schaledb.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/schaledb.py`

 * *Files 2% similar despite different names*

```diff
@@ -511,15 +511,15 @@
 async def draw_fav_li(lvl):
     try:
         stu_li = [
             x
             for x in await schale_get_stu_data()
             if (x["MemoryLobby"] and x["MemoryLobby"][0] == lvl)
         ]
-    except:
+    except Exception:
         logger.exception("获取schale db学生数据失败")
         return "获取SchaleDB学生数据失败，请检查后台输出"
 
     if not stu_li:
         return f"没有学生在羁绊等级{lvl}时解锁L2D"
 
     txt_h = 48
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/gacha.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/data/gacha.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 from typing import Dict, Iterable, List, Optional, TypedDict, Union, cast
 
 import aiofiles
 from nonebot import logger
 from nonebot.adapters.onebot.v11 import MessageSegment
 from pil_utils import BuildImage
 
-from .config import config
-from .data.schaledb import schale_get, schale_get_stu_dict
-from .resource import (
+from ..config import config
+from ..resource import (
     DATA_PATH,
     RES_GACHA_BG,
     RES_GACHA_CARD_BG,
     RES_GACHA_CARD_MASK,
     RES_GACHA_NEW,
     RES_GACHA_PICKUP,
     RES_GACHA_STAR,
     RES_GACHA_STU_ERR,
 )
-from .util import split_list
+from ..util import split_list
+from .schaledb import schale_get, schale_get_stu_dict
 
 GACHA_DATA_PATH = DATA_PATH / "gacha.json"
 if not GACHA_DATA_PATH.exists():
     GACHA_DATA_PATH.write_text("{}")
 
 
 DEFAULT_GACHA_DATA: "GachaData" = {"collected": [], "total_count": 0}
@@ -99,15 +99,15 @@
             stu_j = stu_li[stu.id]
             stu_star: int = stu_j["StarGrade"]
             stu_img = await schale_get(
                 f"images/student/collection/{stu_j['CollectionTexture']}.webp",
                 True,
             )
             stu_img = BuildImage.open(BytesIO(stu_img))
-        except:
+        except Exception:
             logger.exception(f"学生数据获取失败 {stu.id}")
             stu_img = RES_GACHA_STU_ERR
 
         card_img = BuildImage.new("RGBA", RES_GACHA_CARD_MASK.size, (0, 0, 0, 0))
         card_img.image.paste(
             stu_img.resize(RES_GACHA_CARD_MASK.size, keep_ratio=True).image,
             mask=RES_GACHA_CARD_MASK.image,
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/help/__init__.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/help/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/help/manual.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/help/manual.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/help/pic_menu.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/help/pic_menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,9 +64,9 @@
         path = str(get_proper_font("国").path.resolve())
         pic_menu_config.write_text(json.dumps({"default": path}), encoding="u8")
         logger.info("检测到 PicMenu 已加载并且未配置字体，已自动帮您配置系统字体")
 
 
 try:
     set_pic_menu_font()
-except:
+except Exception:
     logger.exception("配置 PicMenu 字体失败")
```

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/__init__.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/calender_banner.png` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/calender_banner.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_bg.png` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_new.png` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_new.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_pickup.png` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_pickup.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_star.png` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_star.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/resource/res/gradient.png` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/resource/res/gradient.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.8.1/nonebot_plugin_bawiki/util.py` & `nonebot_plugin_bawiki-0.8.2/nonebot_plugin_bawiki/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 import datetime
 import json
-from copy import deepcopy
 from dataclasses import dataclass
-from typing import Any, Dict, Iterable, List, Literal, Optional, TypeVar, overload
+from typing import (
+    Any,
+    Dict,
+    Iterable,
+    List,
+    Literal,
+    Optional,
+    TypeVar,
+    Union,
+    cast,
+    overload,
+)
 
 from httpx import AsyncClient
 from nonebot.adapters.onebot.v11 import Message
 from nonebot_plugin_apscheduler import scheduler
 from PIL import Image, ImageOps
 
 from .config import config
 
-_T = TypeVar("_T")
+T = TypeVar("T")
+NestedIterable = Iterable[Union[T, Iterable["NestedIterable[T]"]]]
 
 req_cache: Dict[str, "RequestCache"] = {}
 
 
 @dataclass
 class RequestCache:
     method: str
@@ -179,18 +190,18 @@
     for i, v in enumerate(msgs):
         if isinstance(v, str) and (i != 0):
             v = f"\n{v}"
         im += v
     return im
 
 
-def split_list(li: Iterable[_T], length: int) -> List[List[_T]]:
+def split_list(li: Iterable[T], length: int) -> List[List[T]]:
     latest = []
     tmp = []
     for n, i in enumerate(li):
         tmp.append(i)
         if (n + 1) % length == 0:
-            latest.append(deepcopy(tmp))
-            tmp.clear()
+            latest.append(tmp)
+            tmp = []
     if tmp:
-        latest.append(deepcopy(tmp))
+        latest.append(tmp)
     return latest
```

### Comparing `nonebot_plugin_bawiki-0.8.1/pyproject.toml` & `nonebot_plugin_bawiki-0.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-bawiki"
-version = "0.8.1"
+version = "0.8.2"
 description = "A nonebot2 plugin for Blue Archive."
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.1",
```

### Comparing `nonebot_plugin_bawiki-0.8.1/PKG-INFO` & `nonebot_plugin_bawiki-0.8.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bawiki
-Version: 0.8.1
+Version: 0.8.2
 Summary: A nonebot2 plugin for Blue Archive.
 Keywords: blue archive nonebot nonebot2 bot qq
 Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Communications
@@ -206,14 +206,19 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.8.2
+
+- 修改了 `ba语音` 指令的特性，兼容了有中配语音的学生，请查看该指令帮助获取详细信息
+- 删除了 `arona` 指令模糊搜索展示类别的功能，因为模糊搜索时 `type` 固定为 `0` 了
+
 ### 0.8.1
 
 - 使用 `arona` 指令模糊搜索的时候会显示图片类别了
 
 ### 0.8.0
 
 - 整理项目结构
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.8.1 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.8.2 Summary: A
 nonebot2 plugin for Blue Archive. Keywords: blue archive nonebot nonebot2 bot
 qq Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/ Author-Email:
 student_2333
 126.com> License: MIT Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Communications :: Chat :: ICQ Classifier: Topic :: Games/
 Entertainment Classifier: Topic :: Games/Entertainment :: Board Games
@@ -72,17 +72,22 @@
 (https://lonqie.github.io/SchaleDB/) & [Arona Bot](https://
 doc.arona.diyigemt.com/api/) - æä»¶æ°æ®æºæä¾  ### `bawiki-data`
 æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/bawiki-
 data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
 å®å¨ææ¿ä¸å°½â¦â¦ - [ç±åçµ](https://afdian.net/@lgc2333) -
 èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ ![è®¨é¥­](https://raw.githubusercontent.com/
 lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ###
-0.8.1 - ä½¿ç¨ `arona` æä»¤æ¨¡ç³æç´¢çæ¶åä¼æ¾ç¤ºå¾çç±»å«äº ###
-0.8.0 - æ´çé¡¹ç®ç»æ - æ·»å åç½®å¸®å©æä»¤ `baå¸®å©` - æ·»å  Arona
-Bot æ°æ®æºæä»¤ `arona` - æ·»å äºéç½®é¡¹
+0.8.2 - ä¿®æ¹äº `baè¯­é³`
+æä»¤çç¹æ§ï¼å¼å®¹äºæä¸­éè¯­é³çå­¦çï¼è¯·æ¥çè¯¥æä»¤å¸®å©è·åè¯¦ç»ä¿¡æ¯
+- å é¤äº `arona`
+æä»¤æ¨¡ç³æç´¢å±ç¤ºç±»å«çåè½ï¼å ä¸ºæ¨¡ç³æç´¢æ¶ `type`
+åºå®ä¸º `0` äº ### 0.8.1 - ä½¿ç¨ `arona`
+æä»¤æ¨¡ç³æç´¢çæ¶åä¼æ¾ç¤ºå¾çç±»å«äº ### 0.8.0 -
+æ´çé¡¹ç®ç»æ - æ·»å åç½®å¸®å©æä»¤ `baå¸®å©` - æ·»å  Arona Bot
+æ°æ®æºæä»¤ `arona` - æ·»å äºéç½®é¡¹
 `BA_ARONA_API_URL`ã`BA_ARONA_CDN_URL`ã`BA_CLEAR_REQ_CACHE_INTERVAL`ã`BA_AUTO_CLEAR_ARONA_CACHE`
 - å¶ä»å°æ´æ¹ï¼æ´æ¢ `aiohttp` ä¸º `httpx` ç­ï¼ ### 0.7.10 -
 æ·»å æä»¤ `baå³å¡` ### 0.7.9 - æ·»å éç½®é¡¹ `BA_VOICE_USE_CARD` ###
 0.7.8 - ð NoneBot 2.0 ð ### 0.7.7 - ä¿®å¤ bug ### 0.7.6 -
 ä¿®å¤å¡æ± ä¸ºç©ºä¸ä¼æç¤ºç bug ### 0.7.5 -
 æä»¶å¯ä»¥èªå¨å¸®ä½ éç½® PicMenu çå­ä½äº - ç»æ½å¡æ°å¢äºå·å´
 ### 0.7.2 ~ 0.7.4 - ä¿®å¤ bug ### 0.7.1 - æ´æ¹éç½®é¡¹åç§° ### 0.7.0 -
```

