# Comparing `tmp/dingtalk-stream-0.7.4.tar.gz` & `tmp/dingtalk-stream-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingtalk-stream-0.7.4.tar", last modified: Fri Jul 21 02:07:39 2023, max compression
+gzip compressed data, was "dingtalk-stream-0.7.5.tar", last modified: Fri Jul 21 11:31:28 2023, max compression
```

## Comparing `dingtalk-stream-0.7.4.tar` & `dingtalk-stream-0.7.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:07:39.927550 dingtalk-stream-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-21 02:07:39.927550 dingtalk-stream-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:07:39.927550 dingtalk-stream-0.7.4/dingtalk_stream/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/card_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/card_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/card_replier.py
--rw-r--r--   0 runner    (1001) docker     (123)    25086 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/interactive_card.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:07:39.927550 dingtalk-stream-0.7.4/dingtalk_stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-21 02:07:39.000000 dingtalk-stream-0.7.4/dingtalk_stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-21 02:07:39.000000 dingtalk-stream-0.7.4/dingtalk_stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 02:07:39.000000 dingtalk-stream-0.7.4/dingtalk_stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-21 02:07:39.000000 dingtalk-stream-0.7.4/dingtalk_stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 02:07:39.000000 dingtalk-stream-0.7.4/dingtalk_stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 02:07:39.927550 dingtalk-stream-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:31:28.153699 dingtalk-stream-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-21 11:31:28.153699 dingtalk-stream-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:31:28.153699 dingtalk-stream-0.7.5/dingtalk_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/card_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/card_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/card_replier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25657 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/interactive_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:31:28.153699 dingtalk-stream-0.7.5/dingtalk_stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-21 11:31:28.000000 dingtalk-stream-0.7.5/dingtalk_stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-21 11:31:28.000000 dingtalk-stream-0.7.5/dingtalk_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:31:28.000000 dingtalk-stream-0.7.5/dingtalk_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-21 11:31:28.000000 dingtalk-stream-0.7.5/dingtalk_stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 11:31:28.000000 dingtalk-stream-0.7.5/dingtalk_stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 11:31:28.153699 dingtalk-stream-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/setup.py
```

### Comparing `dingtalk-stream-0.7.4/LICENSE` & `dingtalk-stream-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.4/PKG-INFO` & `dingtalk-stream-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.7.4
+Version: 0.7.5
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.7.4/README.md` & `dingtalk-stream-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.4/dingtalk_stream/__init__.py` & `dingtalk-stream-0.7.5/dingtalk_stream/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from .handlers import EventHandler
 from .handlers import CallbackHandler
 from .handlers import SystemHandler
 from .frames import EventMessage
 from .frames import CallbackMessage
 from .frames import SystemMessage
 from .frames import AckMessage
-from .chatbot import ChatbotMessage, RichTextContent, ImageContent
+from .chatbot import ChatbotMessage, RichTextContent, ImageContent, reply_specified_single_chat, \
+    reply_specified_group_chat
 from .chatbot import TextContent
 from .chatbot import AtUser
 from .chatbot import ChatbotHandler, AsyncChatbotHandler
 from .card_replier import AICardStatus, AICardReplier, CardReplier
-from .card_instance import MarkdownCardInstance, AIMarkdownCardInstance, CarouselCardInstance, MarkdownButtonCardInstance
+from .card_instance import MarkdownCardInstance, AIMarkdownCardInstance, CarouselCardInstance, \
+    MarkdownButtonCardInstance
 from .card_callback import CardCallbackMessage, Card_Callback_Router_Topic
```

### Comparing `dingtalk-stream-0.7.4/dingtalk_stream/card_callback.py` & `dingtalk-stream-0.7.5/dingtalk_stream/card_callback.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.4/dingtalk_stream/card_instance.py` & `dingtalk-stream-0.7.5/dingtalk_stream/card_instance.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.4/dingtalk_stream/card_replier.py` & `dingtalk-stream-0.7.5/dingtalk_stream/card_replier.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             return ""
 
         body = {
             "outTrackId": card_instance_id,
             "userIdType": 1
         }
 
-        # 2：群聊，2：单聊
+        # 2：群聊，1：单聊
         if self.incoming_message.conversation_type == '2':
             body["openSpaceId"] = "dtv1.card//{spaceType}.{spaceId}".format(spaceType="IM_GROUP",
                                                                             spaceId=self.incoming_message.conversation_id)
             body["imGroupOpenDeliverModel"] = {
                 "robotCode": self.dingtalk_client.credential.client_id,
             }
```

### Comparing `dingtalk-stream-0.7.4/dingtalk_stream/chatbot.py` & `dingtalk-stream-0.7.5/dingtalk_stream/chatbot.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,14 +265,34 @@
             self.message_type,
             self.text,
             self.sender_nick,
             self.conversation_title,
         )
 
 
+def reply_specified_single_chat(user_id: str, user_nickname: str = "") -> ChatbotMessage:
+    d = {
+        "senderId": user_id,
+        "senderStaffId": user_id,
+        "sender": user_nickname,
+        "conversationType": '1',
+        "messageId": str(uuid.uuid1()),
+    }
+    return ChatbotMessage.from_dict(d)
+
+
+def reply_specified_group_chat(open_conversation_id: str) -> ChatbotMessage:
+    d = {
+        "conversationId": open_conversation_id,
+        "conversationType": '2',
+        "messageId": str(uuid.uuid1()),
+    }
+    return ChatbotMessage.from_dict(d)
+
+
 class ChatbotHandler(CallbackHandler):
 
     def __init__(self):
         super(ChatbotHandler, self).__init__()
 
     def reply_markdown_card(self, markdown: str, incoming_message: ChatbotMessage, title: str = "", logo: str = "",
                             at_sender: bool = False, at_all: bool = False) -> MarkdownCardInstance:
```

### Comparing `dingtalk-stream-0.7.4/dingtalk_stream/frames.py` & `dingtalk-stream-0.7.5/dingtalk_stream/frames.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.4/dingtalk_stream/handlers.py` & `dingtalk-stream-0.7.5/dingtalk_stream/handlers.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.4/dingtalk_stream/interactive_card.py` & `dingtalk-stream-0.7.5/dingtalk_stream/interactive_card.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.4/dingtalk_stream/stream.py` & `dingtalk-stream-0.7.5/dingtalk_stream/stream.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.4/dingtalk_stream.egg-info/PKG-INFO` & `dingtalk-stream-0.7.5/dingtalk_stream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.7.4
+Version: 0.7.5
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.7.4/dingtalk_stream.egg-info/SOURCES.txt` & `dingtalk-stream-0.7.5/dingtalk_stream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.4/setup.py` & `dingtalk-stream-0.7.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='dingtalk-stream',
-    version='0.7.4',
+    version='0.7.5',
     description='A Python library for sending messages to DingTalk chatbot',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/open-dingtalk/dingtalk-stream-sdk-python',
     author='Ke Jie',
     author_email='jinxi.kj@alibaba-inc.com',
     license='MIT',
```

