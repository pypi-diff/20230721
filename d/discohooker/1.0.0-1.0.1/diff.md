# Comparing `tmp/discohooker-1.0.0.tar.gz` & `tmp/discohooker-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discohooker-1.0.0.tar", last modified: Thu Jul 20 13:44:01 2023, max compression
+gzip compressed data, was "discohooker-1.0.1.tar", last modified: Fri Jul 21 04:48:07 2023, max compression
```

## Comparing `discohooker-1.0.0.tar` & `discohooker-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-20 13:44:01.965225 discohooker-1.0.0/
--rw-r--r--   0 runner    (1000) runner    (1000)     1066 2023-07-17 08:42:29.000000 discohooker-1.0.0/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1298 2023-07-20 13:44:01.965225 discohooker-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      834 2023-07-20 13:43:32.000000 discohooker-1.0.0/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-20 13:44:01.961225 discohooker-1.0.0/discohooker/
--rw-r--r--   0 runner    (1000) runner    (1000)      109 2023-07-20 07:47:04.000000 discohooker-1.0.0/discohooker/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3723 2023-07-20 07:40:11.000000 discohooker-1.0.0/discohooker/embed.py
--rw-r--r--   0 runner    (1000) runner    (1000)      414 2023-07-20 07:39:57.000000 discohooker-1.0.0/discohooker/errors.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2217 2023-07-20 08:58:45.000000 discohooker-1.0.0/discohooker/message.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1191 2023-07-20 12:56:48.000000 discohooker-1.0.0/discohooker/tasks.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2177 2023-07-20 13:07:03.000000 discohooker-1.0.0/discohooker/webhook.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-20 13:44:01.965225 discohooker-1.0.0/discohooker.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1298 2023-07-20 13:44:01.000000 discohooker-1.0.0/discohooker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2023-07-20 13:44:01.000000 discohooker-1.0.0/discohooker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-20 13:44:01.000000 discohooker-1.0.0/discohooker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-07-20 13:44:01.000000 discohooker-1.0.0/discohooker.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-20 13:44:01.000000 discohooker-1.0.0/discohooker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      489 2023-07-20 07:25:45.000000 discohooker-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-20 13:44:01.965225 discohooker-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      712 2023-07-20 13:43:51.000000 discohooker-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-21 04:48:07.171011 discohooker-1.0.1/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1066 2023-07-17 08:42:29.000000 discohooker-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1472 2023-07-21 04:48:07.171011 discohooker-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1008 2023-07-21 04:47:01.000000 discohooker-1.0.1/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-21 04:48:07.167011 discohooker-1.0.1/discohooker/
+-rw-r--r--   0 runner    (1000) runner    (1000)      109 2023-07-20 07:47:04.000000 discohooker-1.0.1/discohooker/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3723 2023-07-20 07:40:11.000000 discohooker-1.0.1/discohooker/embed.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      474 2023-07-21 04:07:46.000000 discohooker-1.0.1/discohooker/errors.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2130 2023-07-21 04:24:57.000000 discohooker-1.0.1/discohooker/message.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      474 2023-07-21 04:24:20.000000 discohooker-1.0.1/discohooker/tasks.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2354 2023-07-21 04:13:53.000000 discohooker-1.0.1/discohooker/webhook.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-21 04:48:07.171011 discohooker-1.0.1/discohooker.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1472 2023-07-21 04:48:06.000000 discohooker-1.0.1/discohooker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2023-07-21 04:48:06.000000 discohooker-1.0.1/discohooker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-21 04:48:06.000000 discohooker-1.0.1/discohooker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-07-21 04:48:06.000000 discohooker-1.0.1/discohooker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-21 04:48:06.000000 discohooker-1.0.1/discohooker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      489 2023-07-20 07:25:45.000000 discohooker-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-21 04:48:07.171011 discohooker-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      712 2023-07-21 04:47:14.000000 discohooker-1.0.1/setup.py
```

### Comparing `discohooker-1.0.0/LICENSE` & `discohooker-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discohooker-1.0.0/PKG-INFO` & `discohooker-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 Metadata-Version: 2.1
 Name: discohooker
-Version: 1.0.0
+Version: 1.0.1
 Summary: A easy PyPI to send Discord Webhook!
 Home-page: https://replit.com/@MAX110331/discohooker
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Quickly Start
+# Quick Start
 ----------------
 **Step 1:**
-> Install Discohooker in Shell.
+> Install [Discohooker](https://pypi.org/project/discohooker/) in Shell.
 > 
 > ```pip install discohooker```
 ----------------
 **Step 2:**
 > Get your Webhook link in [Discord](https://discord.com/channels/@me).
 ---------------
 **Step 3:**
 > Import Discohooker.
 >
 > ```py
 > import discohooker
 > ```
 -------------
 **Step 4:**
-> Setup Webhook.
+> Setup [Webhook](https://discord.com/developers/docs/resources/webhook).
 >
 > ```py
 > webhook=discohooker.Webhook(
 >     weburl="YOUR DISCORD WEBHOOK URL",
 >     name="DISCORD WEBHOOK NAME(IF YOU HAVE SET IN DISCORD ALREADY, YOU MUST NOT ENTER.)",
 >     avatar_url="DISCORD WEBHOOK AVATAR URL(IF YOU HAVE SET IN DISCORD ALREADY, YOU MUST NOT ENTER.)"
 > )
 > ```
 ------------
 **Step 5:**
-> Send Message.
+> Send [Message](https://discord.com/developers/docs/resources/channel#message-object).
 >
 > ```py
 > @discohooker.Tasks.worker
 > async def run():
 >     await webhook.send_message("I am made by Discohooker!")
+> ```
 --------------
 DONE! Do you feel very easy?
```

### Comparing `discohooker-1.0.0/README.md` & `discohooker-1.0.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-# Quickly Start
+# Quick Start
 ----------------
 **Step 1:**
-> Install Discohooker in Shell.
+> Install [Discohooker](https://pypi.org/project/discohooker/) in Shell.
 > 
 > ```pip install discohooker```
 ----------------
 **Step 2:**
 > Get your Webhook link in [Discord](https://discord.com/channels/@me).
 ---------------
 **Step 3:**
 > Import Discohooker.
 >
 > ```py
 > import discohooker
 > ```
 -------------
 **Step 4:**
-> Setup Webhook.
+> Setup [Webhook](https://discord.com/developers/docs/resources/webhook).
 >
 > ```py
 > webhook=discohooker.Webhook(
 >     weburl="YOUR DISCORD WEBHOOK URL",
 >     name="DISCORD WEBHOOK NAME(IF YOU HAVE SET IN DISCORD ALREADY, YOU MUST NOT ENTER.)",
 >     avatar_url="DISCORD WEBHOOK AVATAR URL(IF YOU HAVE SET IN DISCORD ALREADY, YOU MUST NOT ENTER.)"
 > )
 > ```
 ------------
 **Step 5:**
-> Send Message.
+> Send [Message](https://discord.com/developers/docs/resources/channel#message-object).
 >
 > ```py
 > @discohooker.Tasks.worker
 > async def run():
 >     await webhook.send_message("I am made by Discohooker!")
+> ```
 --------------
 DONE! Do you feel very easy?
```

### Comparing `discohooker-1.0.0/discohooker/embed.py` & `discohooker-1.0.1/discohooker/embed.py`

 * *Files identical despite different names*

### Comparing `discohooker-1.0.0/discohooker/message.py` & `discohooker-1.0.1/discohooker/message.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from .errors import Errors
 from .embed import Embed
 from .webhook import Webhook
-import asyncio
 import requests
 
 
 class Message:
     def __init__(self, webhook: Webhook, message_id: int):
         self.webhook=webhook
         response=requests.get(f"{self.webhook.weburl}/messages/{message_id}").json()
@@ -24,32 +23,31 @@
         self.timestamp=response["timestamp"]
         self.mentions_id=[]
         for user in response["mentions"]:
             self.memtions_id.appead(user["id"])
         self.channel_id=response["channel_id"]
 
     
-    async def edit(self, content: str=None, embeds: list[Embed]=[], delete_after: int=None):
+    async def edit(self, content: str=None, embeds: list[Embed]=[]):
         if self.is_sent_by_webhook == False:
-            raise Errors.MessageErro("This message is not sent by this Webhook!")
+            raise Errors.MessageError("This message is not sent by this Webhook!")
         message_id=self.id
         _embeds=[]
         for embed in embeds:
             _embeds.append(embed._to_dict)
         if content == None:
             _content=""
         else:
             _content=content
         _jdata={"content": _content, "embeds": _embeds}
         response=requests.patch(f"{self.weburl}/messages/{message_id}", data=_jdata)
-        if delete_after == None:
+        if response.status_code == 204:
+            raise Errors.APIError("No message's content and embeds have been given by you!")
+        else:
             return response
-        message_id=response.json()["message_id"]
-        await asyncio.sleep(delete_after)
-        return requests.delete(f"{self.weburl}/messages/{message_id}/")
 
 
     async def delete(self):
         if self.is_sent_by_webhook == False:
             raise Errors.MessageErro("This message is not sent by this Webhook!")
         message_id=self.id
         response=requests.delete(f"{self.weburl}/messages/{message_id}")
```

### Comparing `discohooker-1.0.0/discohooker/webhook.py` & `discohooker-1.0.1/discohooker/webhook.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,8 +53,12 @@
         for embed in embeds:
             _embeds.append(embed._to_dict)
         if content == None:
             _content=""
         else:
             _content=content
         _jdata={"content": _content, "embeds": _embeds, "username": self.name, "avatar_url": self.avatar_url}
-        return requests.post(self.weburl, data=_jdata)
+        response=requests.post(self.weburl, data=_jdata)
+        if response.status_code == 204:
+            raise Errors.APIError("No message's content and embeds have been given by you!")
+        else:
+            return response
```

### Comparing `discohooker-1.0.0/discohooker.egg-info/PKG-INFO` & `discohooker-1.0.1/discohooker.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 Metadata-Version: 2.1
 Name: discohooker
-Version: 1.0.0
+Version: 1.0.1
 Summary: A easy PyPI to send Discord Webhook!
 Home-page: https://replit.com/@MAX110331/discohooker
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Quickly Start
+# Quick Start
 ----------------
 **Step 1:**
-> Install Discohooker in Shell.
+> Install [Discohooker](https://pypi.org/project/discohooker/) in Shell.
 > 
 > ```pip install discohooker```
 ----------------
 **Step 2:**
 > Get your Webhook link in [Discord](https://discord.com/channels/@me).
 ---------------
 **Step 3:**
 > Import Discohooker.
 >
 > ```py
 > import discohooker
 > ```
 -------------
 **Step 4:**
-> Setup Webhook.
+> Setup [Webhook](https://discord.com/developers/docs/resources/webhook).
 >
 > ```py
 > webhook=discohooker.Webhook(
 >     weburl="YOUR DISCORD WEBHOOK URL",
 >     name="DISCORD WEBHOOK NAME(IF YOU HAVE SET IN DISCORD ALREADY, YOU MUST NOT ENTER.)",
 >     avatar_url="DISCORD WEBHOOK AVATAR URL(IF YOU HAVE SET IN DISCORD ALREADY, YOU MUST NOT ENTER.)"
 > )
 > ```
 ------------
 **Step 5:**
-> Send Message.
+> Send [Message](https://discord.com/developers/docs/resources/channel#message-object).
 >
 > ```py
 > @discohooker.Tasks.worker
 > async def run():
 >     await webhook.send_message("I am made by Discohooker!")
+> ```
 --------------
 DONE! Do you feel very easy?
```

### Comparing `discohooker-1.0.0/setup.py` & `discohooker-1.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="discohooker",
-    version="1.0.0",
+    version="1.0.1",
     author="MaxPython110331",
     author_email="max.gamil110331@gmail.com",
     description="A easy PyPI to send Discord Webhook!",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://replit.com/@MAX110331/discohooker",
```

