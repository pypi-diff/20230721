# Comparing `tmp/discohooker-1.0.5.tar.gz` & `tmp/discohooker-1.0.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discohooker-1.0.5.tar", last modified: Fri Jul 21 12:54:13 2023, max compression
+gzip compressed data, was "discohooker-1.0.5b1.tar", last modified: Fri Jul 21 07:58:26 2023, max compression
```

## Comparing `discohooker-1.0.5.tar` & `discohooker-1.0.5b1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-21 12:54:13.186044 discohooker-1.0.5/
--rw-r--r--   0 runner    (1000) runner    (1000)     1066 2023-07-17 08:42:29.000000 discohooker-1.0.5/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1472 2023-07-21 12:54:13.186044 discohooker-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1008 2023-07-21 04:47:01.000000 discohooker-1.0.5/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-21 12:54:13.182044 discohooker-1.0.5/discohooker/
--rw-r--r--   0 runner    (1000) runner    (1000)      109 2023-07-20 07:47:04.000000 discohooker-1.0.5/discohooker/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3723 2023-07-20 07:40:11.000000 discohooker-1.0.5/discohooker/embed.py
--rw-r--r--   0 runner    (1000) runner    (1000)      474 2023-07-21 04:07:46.000000 discohooker-1.0.5/discohooker/errors.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2985 2023-07-21 12:51:31.000000 discohooker-1.0.5/discohooker/message.py
--rw-r--r--   0 runner    (1000) runner    (1000)      474 2023-07-21 04:24:20.000000 discohooker-1.0.5/discohooker/tasks.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3387 2023-07-21 07:48:33.000000 discohooker-1.0.5/discohooker/webhook.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-21 12:54:13.186044 discohooker-1.0.5/discohooker.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1472 2023-07-21 12:54:12.000000 discohooker-1.0.5/discohooker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2023-07-21 12:54:12.000000 discohooker-1.0.5/discohooker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-21 12:54:12.000000 discohooker-1.0.5/discohooker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-07-21 12:54:12.000000 discohooker-1.0.5/discohooker.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-21 12:54:12.000000 discohooker-1.0.5/discohooker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      489 2023-07-20 07:25:45.000000 discohooker-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-21 12:54:13.186044 discohooker-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      712 2023-07-21 12:53:53.000000 discohooker-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-21 07:58:26.765497 discohooker-1.0.5b1/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1066 2023-07-17 08:42:29.000000 discohooker-1.0.5b1/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1474 2023-07-21 07:58:26.765497 discohooker-1.0.5b1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1008 2023-07-21 04:47:01.000000 discohooker-1.0.5b1/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-21 07:58:26.757497 discohooker-1.0.5b1/discohooker/
+-rw-r--r--   0 runner    (1000) runner    (1000)      109 2023-07-20 07:47:04.000000 discohooker-1.0.5b1/discohooker/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3723 2023-07-20 07:40:11.000000 discohooker-1.0.5b1/discohooker/embed.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      474 2023-07-21 04:07:46.000000 discohooker-1.0.5b1/discohooker/errors.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3192 2023-07-21 07:57:58.000000 discohooker-1.0.5b1/discohooker/message.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      474 2023-07-21 04:24:20.000000 discohooker-1.0.5b1/discohooker/tasks.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3387 2023-07-21 07:48:33.000000 discohooker-1.0.5b1/discohooker/webhook.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-21 07:58:26.761497 discohooker-1.0.5b1/discohooker.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1474 2023-07-21 07:58:26.000000 discohooker-1.0.5b1/discohooker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2023-07-21 07:58:26.000000 discohooker-1.0.5b1/discohooker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-21 07:58:26.000000 discohooker-1.0.5b1/discohooker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-07-21 07:58:26.000000 discohooker-1.0.5b1/discohooker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-21 07:58:26.000000 discohooker-1.0.5b1/discohooker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      489 2023-07-20 07:25:45.000000 discohooker-1.0.5b1/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-21 07:58:26.765497 discohooker-1.0.5b1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      714 2023-07-21 07:58:18.000000 discohooker-1.0.5b1/setup.py
```

### Comparing `discohooker-1.0.5/LICENSE` & `discohooker-1.0.5b1/LICENSE`

 * *Files identical despite different names*

### Comparing `discohooker-1.0.5/PKG-INFO` & `discohooker-1.0.5b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discohooker
-Version: 1.0.5
+Version: 1.0.5b1
 Summary: A easy PyPI to send Discord Webhook!
 Home-page: https://replit.com/@MAX110331/discohooker
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `discohooker-1.0.5/README.md` & `discohooker-1.0.5b1/README.md`

 * *Files identical despite different names*

### Comparing `discohooker-1.0.5/discohooker/embed.py` & `discohooker-1.0.5b1/discohooker/embed.py`

 * *Files identical despite different names*

### Comparing `discohooker-1.0.5/discohooker/message.py` & `discohooker-1.0.5b1/discohooker/message.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,18 @@
 import requests
 
 
 class Message:
     def __init__(self, webhook: Webhook, message_id: int):
         self.webhook=webhook
         response=requests.get(f"{self.webhook.weburl}/messages/{message_id}").json()
-        try:
-            response["code"]
-        except:
-            pass
+        if response["author"]["id"] == self.webhook.id:
+            self.is_sent_by_webhook=True
         else:
-            raise Errors.MessageNotFound("This message is not sent by webhook so you cannot get this message!")
+            self.is_sent_by_webhook=False
         self.id=response["id"]
         self.content=response["content"]
         self.is_pinned=response["pinned"]
         self.embeds=[]
         for embed in response["embeds"]:
             _embed=Embed()
             _embed._to_dict=embed
@@ -26,14 +24,16 @@
         self.mentions_id=[]
         for user in response["mentions"]:
             self.memtions_id.appead(user["id"])
         self.channel_id=response["channel_id"]
 
     
     async def edit(self, content: str=None, embeds: list[Embed]=[]):
+        if self.is_sent_by_webhook == False:
+            raise Errors.MessageError("This message is not sent by this Webhook!")
         message_id=self.id
         _embeds=[]
         for embed in embeds:
             _embeds.append(embed._to_dict)
         if content == None:
             _content=""
         else:
@@ -57,13 +57,15 @@
         elif response.status_code == 502:
             raise Errors.APIError("There was not a gateway available to process your request. Wait a bit and retry.")
         else:
             return response
 
 
     async def delete(self):
+        if self.is_sent_by_webhook == False:
+            raise Errors.MessageErro("This message is not sent by this Webhook!")
         message_id=self.id
         response=requests.delete(f"{self.webhook.weburl}/messages/{message_id}")
         if response.status_code != 204:
             raise Errors.MessageNotFound("This message was not sent by this Webhook! Please make sure your message id is correct!")
         else:
             return response
```

### Comparing `discohooker-1.0.5/discohooker/webhook.py` & `discohooker-1.0.5b1/discohooker/webhook.py`

 * *Files identical despite different names*

### Comparing `discohooker-1.0.5/discohooker.egg-info/PKG-INFO` & `discohooker-1.0.5b1/discohooker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discohooker
-Version: 1.0.5
+Version: 1.0.5b1
 Summary: A easy PyPI to send Discord Webhook!
 Home-page: https://replit.com/@MAX110331/discohooker
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `discohooker-1.0.5/setup.py` & `discohooker-1.0.5b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="discohooker",
-    version="1.0.5",
+    version="1.0.5b1",
     author="MaxPython110331",
     author_email="max.gamil110331@gmail.com",
     description="A easy PyPI to send Discord Webhook!",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://replit.com/@MAX110331/discohooker",
```

