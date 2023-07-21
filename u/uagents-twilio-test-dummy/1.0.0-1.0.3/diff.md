# Comparing `tmp/uagents_twilio_test_dummy-1.0.0.tar.gz` & `tmp/uagents_twilio_test_dummy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uagents_twilio_test_dummy-1.0.0.tar", max compression
+gzip compressed data, was "uagents_twilio_test_dummy-1.0.3.tar", max compression
```

## Comparing `uagents_twilio_test_dummy-1.0.0.tar` & `uagents_twilio_test_dummy-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1073 2023-07-18 08:13:30.274276 uagents_twilio_test_dummy-1.0.0/LICENSE
--rw-r--r--   0        0        0      576 2023-07-19 05:23:13.567133 uagents_twilio_test_dummy-1.0.0/README.rst
--rw-r--r--   0        0        0      883 2023-07-20 05:12:58.272415 uagents_twilio_test_dummy-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       68 2023-07-19 05:23:14.531167 uagents_twilio_test_dummy-1.0.0/uagents_twilio/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 11:32:55.835669 uagents_twilio_test_dummy-1.0.0/uagents_twilio/gc_integration/__init__.py
--rw-r--r--   0        0        0     1727 2023-07-18 11:32:55.843669 uagents_twilio_test_dummy-1.0.0/uagents_twilio/gc_integration/constants.py
--rw-r--r--   0        0        0    14304 2023-07-19 05:23:14.931181 uagents_twilio_test_dummy-1.0.0/uagents_twilio/gc_integration/google_calendar.py
--rw-r--r--   0        0        0     1229 2023-07-18 11:32:55.847669 uagents_twilio_test_dummy-1.0.0/uagents_twilio/gc_integration/utils.py
--rw-r--r--   0        0        0      125 2023-07-18 08:21:07.874523 uagents_twilio_test_dummy-1.0.0/uagents_twilio/models.py
--rw-r--r--   0        0        0        0 2023-07-18 08:13:30.290264 uagents_twilio_test_dummy-1.0.0/uagents_twilio/protocols/__init__.py
--rw-r--r--   0        0        0     1988 2023-07-19 13:28:23.816363 uagents_twilio_test_dummy-1.0.0/uagents_twilio/protocols/message.py
--rw-r--r--   0        0        0      555 2023-07-19 05:24:13.724857 uagents_twilio_test_dummy-1.0.0/uagents_twilio/webhook.py
--rw-r--r--   0        0        0        0 2023-07-18 08:13:30.286267 uagents_twilio_test_dummy-1.0.0/uagents_twilio/wrappers/__init__.py
--rw-r--r--   0        0        0     1969 2023-07-19 09:32:47.021259 uagents_twilio_test_dummy-1.0.0/uagents_twilio/wrappers/messageWrapper.py
--rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 uagents_twilio_test_dummy-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-18 08:13:30.274276 uagents_twilio_test_dummy-1.0.3/LICENSE
+-rw-r--r--   0        0        0      576 2023-07-19 05:23:13.567133 uagents_twilio_test_dummy-1.0.3/README.rst
+-rw-r--r--   0        0        0      883 2023-07-21 10:29:43.965352 uagents_twilio_test_dummy-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-07-19 05:23:14.531167 uagents_twilio_test_dummy-1.0.3/uagents_twilio/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 11:32:55.835669 uagents_twilio_test_dummy-1.0.3/uagents_twilio/gc_integration/__init__.py
+-rw-r--r--   0        0        0     1727 2023-07-18 11:32:55.843669 uagents_twilio_test_dummy-1.0.3/uagents_twilio/gc_integration/constants.py
+-rw-r--r--   0        0        0    14304 2023-07-19 05:23:14.931181 uagents_twilio_test_dummy-1.0.3/uagents_twilio/gc_integration/google_calendar.py
+-rw-r--r--   0        0        0     1229 2023-07-18 11:32:55.847669 uagents_twilio_test_dummy-1.0.3/uagents_twilio/gc_integration/utils.py
+-rw-r--r--   0        0        0      219 2023-07-21 10:10:13.473269 uagents_twilio_test_dummy-1.0.3/uagents_twilio/models.py
+-rw-r--r--   0        0        0        0 2023-07-18 08:13:30.290264 uagents_twilio_test_dummy-1.0.3/uagents_twilio/protocols/__init__.py
+-rw-r--r--   0        0        0     1432 2023-07-21 10:10:13.621270 uagents_twilio_test_dummy-1.0.3/uagents_twilio/protocols/sms.py
+-rw-r--r--   0        0        0      769 2023-07-21 10:10:13.485269 uagents_twilio_test_dummy-1.0.3/uagents_twilio/webhook.py
+-rw-r--r--   0        0        0        0 2023-07-18 08:13:30.286267 uagents_twilio_test_dummy-1.0.3/uagents_twilio/wrappers/__init__.py
+-rw-r--r--   0        0        0     1969 2023-07-19 09:32:47.021259 uagents_twilio_test_dummy-1.0.3/uagents_twilio/wrappers/smsWrapper.py
+-rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 uagents_twilio_test_dummy-1.0.3/PKG-INFO
```

### Comparing `uagents_twilio_test_dummy-1.0.0/LICENSE` & `uagents_twilio_test_dummy-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uagents_twilio_test_dummy-1.0.0/README.rst` & `uagents_twilio_test_dummy-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `uagents_twilio_test_dummy-1.0.0/pyproject.toml` & `uagents_twilio_test_dummy-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "uagents-twilio-test-dummy"
 #
-version = '1.0.0'
+version = '1.0.3'
 #
 description = ""
 authors = ["Harsh <harsh@gmail.com>"]
 readme = "README.rst"
 repository = "https://github.com/Github User/uagents-twilio"
 packages = [{include = "uagents_twilio"}]
 classifiers=[
```

### Comparing `uagents_twilio_test_dummy-1.0.0/uagents_twilio/gc_integration/constants.py` & `uagents_twilio_test_dummy-1.0.3/uagents_twilio/gc_integration/constants.py`

 * *Files identical despite different names*

### Comparing `uagents_twilio_test_dummy-1.0.0/uagents_twilio/gc_integration/google_calendar.py` & `uagents_twilio_test_dummy-1.0.3/uagents_twilio/gc_integration/google_calendar.py`

 * *Files identical despite different names*

### Comparing `uagents_twilio_test_dummy-1.0.0/uagents_twilio/gc_integration/utils.py` & `uagents_twilio_test_dummy-1.0.3/uagents_twilio/gc_integration/utils.py`

 * *Files identical despite different names*

### Comparing `uagents_twilio_test_dummy-1.0.0/uagents_twilio/protocols/message.py` & `uagents_twilio_test_dummy-1.0.3/uagents_twilio/protocols/sms.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,18 @@
 from decouple import config
 from uagents import Context, Protocol
 
-from uagents_twilio.models import WhatsAppMsg
-from uagents_twilio.wrappers.messageWrapper import WhatsappClient
+from uagents_twilio.models import WhatsAppCustomMsg, WhatsAppWebhookMsg
+from uagents_twilio.wrappers.smsWrapper import WhatsappClient
 
 service_protocol = Protocol()
 
 AGENT1_EMAIL = config("AGENT1_EMAIL")
 AGENT2_EMAIL = config("AGENT2_EMAIL")
 
-# gc = GoogleCalendar(
-#     calendar=AGENT1_EMAIL,
-#     authentication_flow_port=8080,
-#     token_path=token_path,
-# )
-
-# calendar_handler = GCAgentHandler(
-#     agent=service_protocol,
-#     agent_email=AGENT1_EMAIL,
-#     gc=gc,
-#     events_mapping={},
-# )
-
-
 ACCOUNT_SID = config("ACCOUNT_SID")
 AUTH_TOKEN = config("AUTH_TOKEN")
 FROM_NUMBER = config("FROM_NUMBER")
 TO_NUMBER = config("TO_NUMBER")
 
 
 whatsapp_handler = WhatsappClient(
@@ -35,26 +21,22 @@
     account_sid=ACCOUNT_SID,
     auth_token=AUTH_TOKEN,
     from_number=FROM_NUMBER,
     to_number=TO_NUMBER,
 )
 
 
-@service_protocol.on_query(model=WhatsAppMsg)
-async def receive_msg(ctx: Context, sender: str, message: WhatsAppMsg):
-    await ctx.send(sender, WhatsAppMsg(sender=message.sender, msg="Received"))
+@service_protocol.on_query(model=WhatsAppWebhookMsg)
+async def receive_msg(ctx: Context, sender: str, message: WhatsAppWebhookMsg):
+    await ctx.send(sender, WhatsAppWebhookMsg(sender=message.sender, msg="Received"))
+    ctx.storage.set("message", message.msg)
+    whatsapp_handler.send_new_message(message.sender, message.start_message)
+
+
+@service_protocol.on_message(model=WhatsAppCustomMsg)
+async def send_wp_msg(ctx: Context, sender: str, message: WhatsAppCustomMsg):
+    await ctx.send(
+        sender,
+        WhatsAppCustomMsg(receiver=message.receiver, msg="Sending a msg on Whatsapp"),
+    )
     ctx.storage.set("message", message.msg)
-    whatsapp_handler.send_new_message(message.sender, "Success .")
-    # if "fetch" in message.msg:
-    #     print(message.msg)
-    #     event = ctx.storage.get("event")
-    #     event_data = calendar_handler.event_dict(event)
-    #     summary = event["summary"]
-    #     message.msg = summary
-    #     print(message.msg)
-    #     whatsapp_handler.send_new_message(message.sender, f"This is your upcoming event:\n {event_data}\nBy selecting the yes/no option, let me know if you want me to carry out this task.")
-    # elif message.msg == "yes":
-    #     event = ctx.storage.get("event")
-    #     summary = event["summary"]
-    #     message.msg = summary
-    # elif message.msg == "no":
-    #     whatsapp_handler.send_new_message(message.sender, f"How else may I help you?")
+    whatsapp_handler.send_new_message(message.receiver, message.msg)
```

### Comparing `uagents_twilio_test_dummy-1.0.0/uagents_twilio/webhook.py` & `uagents_twilio_test_dummy-1.0.3/uagents_twilio/webhook.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+"""
+This webhook file is just for sample to listen incoming message from twilio and pass it
+to Agenet. Move it to your actual agent project and run it to listen messages.
+"""
 from typing import Annotated
 
 from fastapi import FastAPI, Form
-from models import WhatsAppMsg
+from models import WhatsAppWebhookMsg
 from uagents.query import query
 
 app = FastAPI()
 
 AGENT_ADDRESS = "agent1qfrs3x9eh4pvaymsmwgjkjq4srqq4ctfw8h5hjduscmq4asq027tucn2gqw"
 
 
 @app.post("/incoming")
 async def incoming_message(Body: Annotated[str, Form()], From: Annotated[str, Form()]):
     # Extract relevant information from the incoming message
     print(Body, From)
     await query(
         destination=AGENT_ADDRESS,
-        message=WhatsAppMsg(sender=From, msg=Body),
+        message=WhatsAppWebhookMsg(sender=From, msg=Body, start_message="Success"),
         timeout=10,
     )
```

### Comparing `uagents_twilio_test_dummy-1.0.0/uagents_twilio/wrappers/messageWrapper.py` & `uagents_twilio_test_dummy-1.0.3/uagents_twilio/wrappers/smsWrapper.py`

 * *Files identical despite different names*

### Comparing `uagents_twilio_test_dummy-1.0.0/PKG-INFO` & `uagents_twilio_test_dummy-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uagents-twilio-test-dummy
-Version: 1.0.0
+Version: 1.0.3
 Summary: 
 Home-page: https://github.com/Github User/uagents-twilio
 Author: Harsh
 Author-email: harsh@gmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

