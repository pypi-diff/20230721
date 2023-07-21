# Comparing `tmp/nonebot_plugin_game_collection-2.3.8.tar.gz` & `tmp/nonebot_plugin_game_collection-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-2.3.8.tar", last modified: Sat Jul 15 10:42:35 2023, max compression
+gzip compressed data, was "nonebot_plugin_game_collection-2.3.9.tar", last modified: Sat Jul 15 12:12:47 2023, max compression
```

## Comparing `nonebot_plugin_game_collection-2.3.8.tar` & `nonebot_plugin_game_collection-2.3.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 10:42:35.360696 nonebot_plugin_game_collection-2.3.8/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.3.8/LICENSE
--rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0      376 2023-07-15 10:42:35.360195 nonebot_plugin_game_collection-2.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 10:42:35.299018 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/
--rw-rw-rw-   0        0        0    21797 2023-07-15 10:39:13.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/Account.py
--rw-rw-rw-   0        0        0     2692 2023-07-11 15:32:39.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/Alchemy.py
-drwxrwxrwx   0        0        0        0 2023-07-15 10:42:35.310776 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/Fortress/
--rw-rw-rw-   0        0        0    10093 2023-07-02 07:42:47.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/Fortress/core.py
--rw-rw-rw-   0        0        0    73450 2023-07-15 06:50:16.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/Game.py
-drwxrwxrwx   0        0        0        0 2023-07-15 10:42:35.319372 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/HorseRace/
--rw-rw-rw-   0        0        0    15602 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/HorseRace/events_main.py
--rw-rw-rw-   0        0        0     6399 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/HorseRace/horse.py
--rw-rw-rw-   0        0        0     5151 2023-07-01 10:30:51.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/HorseRace/race_group.py
--rw-rw-rw-   0        0        0     9182 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/HorseRace/start.py
--rw-rw-rw-   0        0        0    10601 2023-07-15 04:46:14.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/Manager.py
--rw-rw-rw-   0        0        0    24131 2023-07-15 09:45:15.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/Market.py
--rw-rw-rw-   0        0        0    23596 2023-07-07 16:48:24.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/Prop.py
--rw-rw-rw-   0        0        0    33417 2023-07-15 09:37:07.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/__init__.py
--rw-rw-rw-   0        0        0     3733 2023-07-11 14:30:16.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/config.py
--rw-rw-rw-   0        0        0    12289 2023-07-15 09:28:04.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/data.py
-drwxrwxrwx   0        0        0        0 2023-07-15 10:42:35.322373 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/
-drwxrwxrwx   0        0        0        0 2023-07-15 10:42:35.347036 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/horserace/
--rw-rw-rw-   0        0        0     5488 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/horserace/Stand.json
--rw-rw-rw-   0        0        0     4549 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
--rw-rw-rw-   0        0        0     1757 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
--rw-rw-rw-   0        0        0      906 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/horserace/基础事件.json
--rw-rw-rw-   0        0        0     2717 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
--rw-rw-rw-   0        0        0     1257 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
--rw-rw-rw-   0        0        0    22637 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/horserace/群友日常.json
--rw-rw-rw-   0        0        0     4751 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
--rw-rw-rw-   0        0        0     1010 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
--rw-rw-rw-   0        0        0     2253 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
--rw-rw-rw-   0        0        0    12889 2023-07-11 16:50:54.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/menu_data.json
--rw-rw-rw-   0        0        0     5332 2023-07-07 16:19:38.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/props_library.json
-drwxrwxrwx   0        0        0        0 2023-07-15 10:42:35.348538 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/subprocess/
--rw-rw-rw-   0        0        0     2278 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
-drwxrwxrwx   0        0        0        0 2023-07-15 10:42:35.358193 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/utils/
--rw-rw-rw-   0        0        0     1323 2023-06-27 06:06:09.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/utils/avatar.py
--rw-rw-rw-   0        0        0    22338 2023-07-14 15:16:16.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/utils/chart.py
--rw-rw-rw-   0        0        0     1141 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-15 10:42:35.309275 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection.egg-info/
--rw-rw-rw-   0        0        0      376 2023-07-15 10:42:35.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1976 2023-07-15 10:42:35.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 10:42:35.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-07-15 10:42:35.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-07-15 10:42:35.000000 nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 10:42:35.360696 nonebot_plugin_game_collection-2.3.8/setup.cfg
--rw-rw-rw-   0        0        0      730 2023-07-15 10:42:31.000000 nonebot_plugin_game_collection-2.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 12:12:47.164721 nonebot_plugin_game_collection-2.3.9/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.3.9/LICENSE
+-rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      376 2023-07-15 12:12:47.164220 nonebot_plugin_game_collection-2.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 12:12:47.112839 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/
+-rw-rw-rw-   0        0        0    21808 2023-07-15 12:09:39.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/Account.py
+-rw-rw-rw-   0        0        0     2692 2023-07-11 15:32:39.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/Alchemy.py
+drwxrwxrwx   0        0        0        0 2023-07-15 12:12:47.122847 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/Fortress/
+-rw-rw-rw-   0        0        0    10093 2023-07-02 07:42:47.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/Fortress/core.py
+-rw-rw-rw-   0        0        0    73450 2023-07-15 06:50:16.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/Game.py
+drwxrwxrwx   0        0        0        0 2023-07-15 12:12:47.130854 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/HorseRace/
+-rw-rw-rw-   0        0        0    15602 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/HorseRace/events_main.py
+-rw-rw-rw-   0        0        0     6399 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/HorseRace/horse.py
+-rw-rw-rw-   0        0        0     5151 2023-07-01 10:30:51.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/HorseRace/race_group.py
+-rw-rw-rw-   0        0        0     9182 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/HorseRace/start.py
+-rw-rw-rw-   0        0        0    10601 2023-07-15 04:46:14.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/Manager.py
+-rw-rw-rw-   0        0        0    24131 2023-07-15 09:45:15.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/Market.py
+-rw-rw-rw-   0        0        0    23596 2023-07-07 16:48:24.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/Prop.py
+-rw-rw-rw-   0        0        0    33417 2023-07-15 09:37:07.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/__init__.py
+-rw-rw-rw-   0        0        0     3733 2023-07-11 14:30:16.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/config.py
+-rw-rw-rw-   0        0        0    12289 2023-07-15 09:28:04.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/data.py
+drwxrwxrwx   0        0        0        0 2023-07-15 12:12:47.134402 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/
+drwxrwxrwx   0        0        0        0 2023-07-15 12:12:47.154416 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/horserace/
+-rw-rw-rw-   0        0        0     5488 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/horserace/Stand.json
+-rw-rw-rw-   0        0        0     4549 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
+-rw-rw-rw-   0        0        0     1757 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
+-rw-rw-rw-   0        0        0      906 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/horserace/基础事件.json
+-rw-rw-rw-   0        0        0     2717 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
+-rw-rw-rw-   0        0        0     1257 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
+-rw-rw-rw-   0        0        0    22637 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/horserace/群友日常.json
+-rw-rw-rw-   0        0        0     4751 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
+-rw-rw-rw-   0        0        0     1010 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
+-rw-rw-rw-   0        0        0     2253 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
+-rw-rw-rw-   0        0        0    12889 2023-07-11 16:50:54.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/menu_data.json
+-rw-rw-rw-   0        0        0     5332 2023-07-07 16:19:38.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/props_library.json
+drwxrwxrwx   0        0        0        0 2023-07-15 12:12:47.155917 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/subprocess/
+-rw-rw-rw-   0        0        0     2278 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
+drwxrwxrwx   0        0        0        0 2023-07-15 12:12:47.162218 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/utils/
+-rw-rw-rw-   0        0        0     1323 2023-06-27 06:06:09.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/utils/avatar.py
+-rw-rw-rw-   0        0        0    22338 2023-07-14 15:16:16.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/utils/chart.py
+-rw-rw-rw-   0        0        0     1141 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-15 12:12:47.121346 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-07-15 12:12:46.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1976 2023-07-15 12:12:47.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 12:12:46.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-07-15 12:12:46.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-07-15 12:12:46.000000 nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 12:12:47.165221 nonebot_plugin_game_collection-2.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      730 2023-07-15 12:12:36.000000 nonebot_plugin_game_collection-2.3.9/setup.py
```

### Comparing `nonebot_plugin_game_collection-2.3.8/LICENSE` & `nonebot_plugin_game_collection-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/README.md` & `nonebot_plugin_game_collection-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/Account.py` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/Account.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,18 +146,20 @@
             company.stock += group_account.stocks[company_id]
             del group_account.stocks[company_id]
         i += 0.1
         j = i**2
     for user_id in group.namelist:
         user_data[user_id].group_accounts[group_id].revolution = False
     company = group.company
-    if company.level:
-        company.level += 1
-        company.issuance = 20000*company.level
-        company.bank = int(company.bank * Manager.group_wealths(group_id)/group_gold)
+    level = company.level
+    if level:
+        level += 1
+        company.level = level
+        company.issuance = 20000*level
+        company.bank = int(company.bank * (level - 1) / level)
     data.save()
     return f"重置成功！恭喜{first_name}进入挂件榜☆！\n当前系数为：{round(gini,3)}，重置签到已刷新。"
 
 def transfer_gold(event:GroupMessageEvent, target:Tuple[UserDict,GroupAccount], gold:int) -> str:
     """
     转账处理
         param:
```

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/Alchemy.py` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/Alchemy.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/Fortress/core.py` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/Fortress/core.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/Game.py` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/Game.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/HorseRace/events_main.py` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/HorseRace/events_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/HorseRace/horse.py` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/HorseRace/horse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/HorseRace/race_group.py` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/HorseRace/race_group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/HorseRace/start.py` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/HorseRace/start.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/Manager.py` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/Manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/Market.py` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/Market.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/Prop.py` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/Prop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/__init__.py` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/config.py` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/data.py` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/horserace/Stand.json` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/horserace/Stand.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/horserace/基础事件.json` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/horserace/基础事件.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/horserace/群友日常.json` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/horserace/群友日常.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/menu_data.json` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/menu_data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/props_library.json` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/props_library.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/resource/subprocess/ohlc.py` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/resource/subprocess/ohlc.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/utils/avatar.py` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/utils/chart.py` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/utils/chart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection/utils/utils.py` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/nonebot_plugin_game_collection.egg-info/SOURCES.txt` & `nonebot_plugin_game_collection-2.3.9/nonebot_plugin_game_collection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.8/setup.py` & `nonebot_plugin_game_collection-2.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_game_collection',
-version='2.3.8',
+version='2.3.9',
 description='改自nonebot_plugin_russian合并了nonebot_plugin_horserace还有一些自编玩法的小游戏合集。',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_game_collection","nonebot_plugin_game_collection.*"]),
```

