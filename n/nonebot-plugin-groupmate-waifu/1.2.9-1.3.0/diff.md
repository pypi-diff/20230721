# Comparing `tmp/nonebot_plugin_groupmate_waifu-1.2.9.tar.gz` & `tmp/nonebot_plugin_groupmate_waifu-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_groupmate_waifu-1.2.9.tar", last modified: Fri Jul 21 12:57:26 2023, max compression
+gzip compressed data, was "nonebot_plugin_groupmate_waifu-1.3.0.tar", last modified: Fri Jul 21 13:42:21 2023, max compression
```

## Comparing `nonebot_plugin_groupmate_waifu-1.2.9.tar` & `nonebot_plugin_groupmate_waifu-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 12:57:26.346466 nonebot_plugin_groupmate_waifu-1.2.9/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_groupmate_waifu-1.2.9/LICENSE
--rw-rw-rw-   0        0        0      279 2023-07-21 12:57:26.345965 nonebot_plugin_groupmate_waifu-1.2.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-21 12:57:26.332747 nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu/
--rw-rw-rw-   0        0        0    21887 2023-07-21 12:53:08.000000 nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu/__init__.py
--rw-rw-rw-   0        0        0      354 2023-07-17 15:11:43.000000 nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu/config.py
--rw-rw-rw-   0        0        0     2015 2023-07-21 12:53:08.000000 nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 12:57:26.344463 nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu.egg-info/
--rw-rw-rw-   0        0        0      279 2023-07-21 12:57:26.000000 nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-07-21 12:57:26.000000 nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 12:57:26.000000 nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-07-21 12:57:26.000000 nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-07-21 12:57:26.000000 nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 12:57:26.346966 nonebot_plugin_groupmate_waifu-1.2.9/setup.cfg
--rw-rw-rw-   0        0        0      567 2023-07-21 12:57:21.000000 nonebot_plugin_groupmate_waifu-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:42:21.307841 nonebot_plugin_groupmate_waifu-1.3.0/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_groupmate_waifu-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0      279 2023-07-21 13:42:21.306338 nonebot_plugin_groupmate_waifu-1.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-21 13:42:21.289662 nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu/
+-rw-rw-rw-   0        0        0    21763 2023-07-21 13:35:00.000000 nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu/__init__.py
+-rw-rw-rw-   0        0        0      354 2023-07-17 15:11:43.000000 nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu/config.py
+-rw-rw-rw-   0        0        0     2015 2023-07-21 12:53:08.000000 nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:42:21.302394 nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-07-21 13:42:21.000000 nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-07-21 13:42:21.000000 nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 13:42:21.000000 nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-07-21 13:42:21.000000 nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-07-21 13:42:21.000000 nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 13:42:21.307841 nonebot_plugin_groupmate_waifu-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      567 2023-07-21 13:42:16.000000 nonebot_plugin_groupmate_waifu-1.3.0/setup.py
```

### Comparing `nonebot_plugin_groupmate_waifu-1.2.9/LICENSE` & `nonebot_plugin_groupmate_waifu-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu/__init__.py` & `nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,24 +268,28 @@
                     msg = "你已经有CP了，不许花心哦~" + MessageSegment.image(file = await user_img(waifu_id)) + f"你的CP：{member['card'] or member['nickname']}"
             else:
                 msg = tips + MessageSegment.image(file = await user_img(waifu_id)) + f"『{member['card'] or member['nickname']}』！"
             await bot.send(event,msg,at_sender = True)
             return False
 
     if at:
-        tips = "恭喜你娶到了群友!\n" + tips
         if at == rec.get(at):
-            waifu_id = at
+            X = HE
             del rec[waifu_id]
         else:
             X = random.randint(1,100)
-            if 0 < X <= HE:
-                waifu_id = at
-            elif HE < X <= BE:
-                waifu_id = user_id
+
+        if 0 < X <= HE:
+            waifu_id = at
+            tips = "恭喜你娶到了群友!\n" + tips
+        elif HE < X <= BE:
+            waifu_id = user_id
+        else:
+            pass
+
     if not waifu_id:
         group_id = event.group_id
         member_list = await bot.get_group_member_list(group_id = group_id)
         lastmonth = event.time - last_sent_time_filter
         id_list = {member['user_id'] for member in member_list if member["last_sent_time"] > lastmonth}
         waifu_ids = id_list - set(rec.keys())
         waifu_ids -= protect_set
@@ -312,25 +316,24 @@
     rec = record_CP.setdefault(group_id,{})
     waifu_set = record_waifu.setdefault(group_id,set())
     if waifu_id in rec:
         waifu_cp = rec[waifu_id]
         member = await bot.get_group_member_info(group_id = group_id, user_id = waifu_cp)
         msg = "人家已经名花有主了~" + MessageSegment.image(file = await user_img(waifu_cp)) + "ta的cp：" + (member['card'] or member['nickname'])
         if waifu_id in record_lock.get(group_id,{}).keys():
-            if random.randint(1,100) > NTR: 
-                record_CP[group_id][user_id] = user_id
             await waifu.finish(msg + "\n本对cp已锁！",at_sender = True)
-        elif random.randint(1,100) <= NTR: # 彩蛋
+        X = random.randint(1,100)
+        if X > NTR:
+            record_CP[group_id][user_id] = user_id
+        else:
             rec.pop(waifu_cp)
             waifu_set.discard(waifu_cp)
-            await waifu.send(msg + "\n但是...",at_sender = True)
-        else:
-            record_CP[group_id][user_id] = user_id
-            await waifu.finish(msg,at_sender = True)
-        await asyncio.sleep(1)
+            await waifu.send(msg + "\n但是...",at_sender = True)        
+            await asyncio.sleep(1)
+
     record_CP[group_id][user_id] = waifu_id
     record_CP[group_id][waifu_id] = user_id
     waifu_set.add(waifu_id)
     member = await bot.get_group_member_info(group_id = group_id, user_id = waifu_id)
     msg = tips + MessageSegment.image(file = await user_img(waifu_id)) + f"『{(member['card'] or member['nickname'])}』！"
     save(record_waifu_file,record_waifu)
     save(record_CP_file,record_CP)
```

### Comparing `nonebot_plugin_groupmate_waifu-1.2.9/nonebot_plugin_groupmate_waifu/utils.py` & `nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_groupmate_waifu-1.2.9/setup.py` & `nonebot_plugin_groupmate_waifu-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_groupmate_waifu',
-version='1.2.9',
+version='1.3.0',
 description='娶群友',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_groupmate_waifu"]),
```

