# Comparing `tmp/whatsapp-chatbot-python-0.5.2.tar.gz` & `tmp/whatsapp-chatbot-python-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-chatbot-python-0.5.2.tar", last modified: Fri Jul 14 05:42:14 2023, max compression
+gzip compressed data, was "whatsapp-chatbot-python-0.5.3.tar", last modified: Fri Jul 21 05:38:42 2023, max compression
```

## Comparing `whatsapp-chatbot-python-0.5.2.tar` & `whatsapp-chatbot-python-0.5.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 05:42:14.956021 whatsapp-chatbot-python-0.5.2/
--rw-rw-rw-   0        0        0    18829 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/LICENSE
--rw-rw-rw-   0        0        0    15842 2023-07-14 05:42:14.955019 whatsapp-chatbot-python-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0    14404 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-14 05:42:14.956021 whatsapp-chatbot-python-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1809 2023-07-14 05:23:03.000000 whatsapp-chatbot-python-0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:42:14.941969 whatsapp-chatbot-python-0.5.2/tests/
--rw-rw-rw-   0        0        0     1459 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/tests/test_manager.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:42:14.943990 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/
--rw-rw-rw-   0        0        0      270 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/__init__.py
--rw-rw-rw-   0        0        0     1931 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/bot.py
--rw-rw-rw-   0        0        0     4091 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/filters.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:42:14.954016 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/manager/
--rw-rw-rw-   0        0        0        0 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/manager/__init__.py
--rw-rw-rw-   0        0        0     4513 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/manager/handler.py
--rw-rw-rw-   0        0        0     2022 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/manager/observer.py
--rw-rw-rw-   0        0        0     1144 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/manager/router.py
--rw-rw-rw-   0        0        0     2643 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/manager/state.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:42:14.949003 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python.egg-info/
--rw-rw-rw-   0        0        0    15842 2023-07-14 05:42:14.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      598 2023-07-14 05:42:14.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 05:42:14.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-07-14 05:42:14.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-07-14 05:42:14.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 05:38:42.443641 whatsapp-chatbot-python-0.5.3/
+-rw-rw-rw-   0        0        0    18829 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.3/LICENSE
+-rw-rw-rw-   0        0        0    15842 2023-07-21 05:38:42.443641 whatsapp-chatbot-python-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0    14404 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-21 05:38:42.443641 whatsapp-chatbot-python-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1809 2023-07-21 05:37:30.000000 whatsapp-chatbot-python-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 05:38:42.430608 whatsapp-chatbot-python-0.5.3/tests/
+-rw-rw-rw-   0        0        0     1459 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.3/tests/test_manager.py
+drwxrwxrwx   0        0        0        0 2023-07-21 05:38:42.432612 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/
+-rw-rw-rw-   0        0        0      270 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/__init__.py
+-rw-rw-rw-   0        0        0     1931 2023-07-20 12:30:27.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/bot.py
+-rw-rw-rw-   0        0        0     4362 2023-07-21 05:35:42.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/filters.py
+drwxrwxrwx   0        0        0        0 2023-07-21 05:38:42.441636 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/manager/
+-rw-rw-rw-   0        0        0        0 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/manager/__init__.py
+-rw-rw-rw-   0        0        0     4595 2023-07-21 05:35:42.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/manager/handler.py
+-rw-rw-rw-   0        0        0     2022 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/manager/observer.py
+-rw-rw-rw-   0        0        0     1144 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/manager/router.py
+-rw-rw-rw-   0        0        0     2643 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/manager/state.py
+drwxrwxrwx   0        0        0        0 2023-07-21 05:38:42.437627 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python.egg-info/
+-rw-rw-rw-   0        0        0    15842 2023-07-21 05:38:42.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      598 2023-07-21 05:38:42.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 05:38:42.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-21 05:38:42.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-07-21 05:38:42.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python.egg-info/top_level.txt
```

### Comparing `whatsapp-chatbot-python-0.5.2/LICENSE` & `whatsapp-chatbot-python-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.2/PKG-INFO` & `whatsapp-chatbot-python-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chatbot-python
-Version: 0.5.2
+Version: 0.5.3
 Summary: This library helps you easily create a Python chatbot with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-chatbot-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `whatsapp-chatbot-python-0.5.2/README.md` & `whatsapp-chatbot-python-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.2/setup.py` & `whatsapp-chatbot-python-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="whatsapp-chatbot-python",
-    version="0.5.2",
+    version="0.5.3",
     description=(
         "This library helps you easily create"
         " a Python chatbot with WhatsApp API."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="GREEN API",
```

### Comparing `whatsapp-chatbot-python-0.5.2/tests/test_manager.py` & `whatsapp-chatbot-python-0.5.3/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/bot.py` & `whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/bot.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/filters.py` & `whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,26 +62,30 @@
     def __init__(self, text_message: Union[str, List[str]]):
         self.text_message = text_message
         if isinstance(text_message, str):
             self.text_message = [text_message]
 
     def check_event(self, notification: "Notification") -> bool:
         text_message = notification.message_text
+        if text_message is None:
+            return False
 
         if text_message in self.text_message:
             return True
         return False
 
 
 class RegExpFilter(AbstractFilter):
     def __init__(self, pattern: str):
         self.pattern = pattern
 
     def check_event(self, notification: "Notification") -> bool:
         text_message = notification.message_text
+        if text_message is None:
+            return False
 
         if fullmatch(self.pattern, text_message):
             return True
         return False
 
 
 class CommandFilter(AbstractFilter):
@@ -91,14 +95,16 @@
             self.prefixes = prefixes
         elif isinstance(command, tuple):
             if len(command) == 2:
                 self.command, self.prefixes = command
 
     def check_event(self, notification: "Notification") -> bool:
         text_message = notification.message_text
+        if text_message is None:
+            return False
 
         for prefix in self.prefixes:
             if text_message.split()[0] != f"{prefix}{self.command}":
                 continue
             return True
         return False
 
@@ -127,18 +133,21 @@
     "type_message": TypeMessageFilter,
     "text_message": TextMessageFilter,
     "regexp": RegExpFilter,
     "command": CommandFilter,
     "state": StateFilter
 }
 
+TEXT_TYPES = ["textMessage", "extendedTextMessage", "quotedMessage"]
+
 __all__ = [
     "AbstractFilter",
     "ChatIDFilter",
     "SenderFilter",
     "TypeMessageFilter",
     "TextMessageFilter",
     "RegExpFilter",
     "CommandFilter",
     "StateFilter",
-    "filters"
+    "filters",
+    "TEXT_TYPES"
 ]
```

### Comparing `whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/manager/handler.py` & `whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/manager/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,18 @@
 
     def get_message_text(self) -> Optional[str]:
         message_data = self.event["messageData"]
 
         type_message = message_data["typeMessage"]
         if type_message == "textMessage":
             return message_data["textMessageData"]["textMessage"]
-        elif type_message == "extendedTextMessage":
+        elif (
+                type_message == "extendedTextMessage"
+                or type_message == "quotedMessage"
+        ):
             return message_data["extendedTextMessageData"]["text"]
 
     def answer(
             self,
             message: str,
             quoted_message_id: Optional[str] = None,
             archive_chat: Optional[bool] = None,
```

### Comparing `whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/manager/observer.py` & `whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/manager/observer.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/manager/router.py` & `whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/manager/router.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/manager/state.py` & `whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/manager/state.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python.egg-info/PKG-INFO` & `whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chatbot-python
-Version: 0.5.2
+Version: 0.5.3
 Summary: This library helps you easily create a Python chatbot with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-chatbot-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python.egg-info/SOURCES.txt` & `whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

