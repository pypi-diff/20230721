# Comparing `tmp/asynccore-1.2.0.tar.gz` & `tmp/asynccore-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asynccore-1.2.0.tar", last modified: Sat Jul  8 15:52:34 2023, max compression
+gzip compressed data, was "asynccore-1.2.1.tar", last modified: Fri Jul 21 10:40:13 2023, max compression
```

## Comparing `asynccore-1.2.0.tar` & `asynccore-1.2.1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 15:52:34.519277 asynccore-1.2.0/
--rw-rw-rw-   0        0        0     2110 2023-07-08 15:52:34.518277 asynccore-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1506 2023-07-06 19:37:41.000000 asynccore-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 15:52:34.454277 asynccore-1.2.0/asynccore/
--rw-rw-rw-   0        0        0      558 2023-07-05 21:04:10.000000 asynccore-1.2.0/asynccore/__init__.py
--rw-rw-rw-   0        0        0      456 2023-07-06 17:17:18.000000 asynccore-1.2.0/asynccore/__main__.py
--rw-rw-rw-   0        0        0     1842 2023-07-06 19:07:51.000000 asynccore-1.2.0/asynccore/activity.py
--rw-rw-rw-   0        0        0    15034 2023-07-06 18:48:51.000000 asynccore-1.2.0/asynccore/cache.py
--rw-rw-rw-   0        0        0    22946 2023-07-06 17:17:18.000000 asynccore-1.2.0/asynccore/client.py
-drwxrwxrwx   0        0        0        0 2023-07-08 15:52:34.486277 asynccore-1.2.0/asynccore/commands/
--rw-rw-rw-   0        0        0      141 2023-07-02 18:28:20.000000 asynccore-1.2.0/asynccore/commands/__init__.py
--rw-rw-rw-   0        0        0     5881 2023-07-05 21:02:29.000000 asynccore-1.2.0/asynccore/commands/application.py
--rw-rw-rw-   0        0        0     7576 2023-07-06 19:11:25.000000 asynccore-1.2.0/asynccore/commands/slashcommands.py
--rw-rw-rw-   0        0        0     7667 2023-07-04 22:44:09.000000 asynccore-1.2.0/asynccore/components.py
--rw-rw-rw-   0        0        0     1826 2023-07-02 19:16:30.000000 asynccore-1.2.0/asynccore/enums.py
--rw-rw-rw-   0        0        0     1116 2023-07-02 18:42:43.000000 asynccore-1.2.0/asynccore/errors.py
-drwxrwxrwx   0        0        0        0 2023-07-08 15:52:34.518277 asynccore-1.2.0/asynccore/gateway/
--rw-rw-rw-   0        0        0      238 2023-07-02 18:06:21.000000 asynccore-1.2.0/asynccore/gateway/__init__.py
--rw-rw-rw-   0        0        0      662 2023-07-02 18:23:21.000000 asynccore-1.2.0/asynccore/gateway/enums.py
--rw-rw-rw-   0        0        0      878 2023-07-03 01:42:17.000000 asynccore-1.2.0/asynccore/gateway/errors.py
--rw-rw-rw-   0        0        0     5016 2023-07-05 20:45:36.000000 asynccore-1.2.0/asynccore/gateway/event.py
--rw-rw-rw-   0        0        0    14786 2023-07-05 21:04:10.000000 asynccore-1.2.0/asynccore/gateway/gateway.py
--rw-rw-rw-   0        0        0     1981 2023-07-06 17:56:48.000000 asynccore-1.2.0/asynccore/gateway/response.py
--rw-rw-rw-   0        0        0    10340 2023-07-06 18:07:33.000000 asynccore-1.2.0/asynccore/http.py
--rw-rw-rw-   0        0        0      868 2023-07-02 18:40:30.000000 asynccore-1.2.0/asynccore/logger.py
--rw-rw-rw-   0        0        0      593 2023-07-02 18:40:37.000000 asynccore-1.2.0/asynccore/permissionbuilder.py
--rw-rw-rw-   0        0        0     2713 2023-07-02 18:36:58.000000 asynccore-1.2.0/asynccore/tasks.py
--rw-rw-rw-   0        0        0      455 2023-07-02 18:36:30.000000 asynccore-1.2.0/asynccore/typings.py
--rw-rw-rw-   0        0        0    33855 2023-07-05 21:10:25.000000 asynccore-1.2.0/asynccore/user.py
-drwxrwxrwx   0        0        0        0 2023-07-08 15:52:34.470277 asynccore-1.2.0/asynccore.egg-info/
--rw-rw-rw-   0        0        0     2110 2023-07-08 15:52:34.000000 asynccore-1.2.0/asynccore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      764 2023-07-08 15:52:34.000000 asynccore-1.2.0/asynccore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 15:52:34.000000 asynccore-1.2.0/asynccore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-07-08 15:52:34.000000 asynccore-1.2.0/asynccore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-08 15:52:34.000000 asynccore-1.2.0/asynccore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      585 2023-07-03 00:26:09.000000 asynccore-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-08 15:52:34.519277 asynccore-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1253 2023-07-08 15:51:06.000000 asynccore-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 10:40:13.832469 asynccore-1.2.1/
+-rw-rw-rw-   0        0        0     1083 2023-07-21 10:34:53.000000 asynccore-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2786 2023-07-21 10:40:13.832469 asynccore-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2143 2023-07-21 10:34:53.000000 asynccore-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 10:40:13.807553 asynccore-1.2.1/asynccore/
+-rw-rw-rw-   0        0        0      590 2023-07-13 02:14:38.000000 asynccore-1.2.1/asynccore/__init__.py
+-rw-rw-rw-   0        0        0      422 2023-07-13 02:00:35.000000 asynccore-1.2.1/asynccore/__main__.py
+-rw-rw-rw-   0        0        0     1794 2023-07-13 02:00:35.000000 asynccore-1.2.1/asynccore/activity.py
+-rw-rw-rw-   0        0        0    15319 2023-07-21 10:27:15.000000 asynccore-1.2.1/asynccore/cache.py
+-rw-rw-rw-   0        0        0    23544 2023-07-21 10:30:13.000000 asynccore-1.2.1/asynccore/client.py
+drwxrwxrwx   0        0        0        0 2023-07-21 10:40:13.828482 asynccore-1.2.1/asynccore/commands/
+-rw-rw-rw-   0        0        0      141 2023-07-02 18:28:20.000000 asynccore-1.2.1/asynccore/commands/__init__.py
+-rw-rw-rw-   0        0        0     6302 2023-07-13 02:41:35.000000 asynccore-1.2.1/asynccore/commands/application.py
+-rw-rw-rw-   0        0        0     7692 2023-07-13 02:44:22.000000 asynccore-1.2.1/asynccore/commands/slashcommands.py
+-rw-rw-rw-   0        0        0     7928 2023-07-13 02:08:32.000000 asynccore-1.2.1/asynccore/components.py
+-rw-rw-rw-   0        0        0     1848 2023-07-13 02:14:40.000000 asynccore-1.2.1/asynccore/enums.py
+-rw-rw-rw-   0        0        0     1142 2023-07-13 02:37:48.000000 asynccore-1.2.1/asynccore/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-21 10:40:13.831472 asynccore-1.2.1/asynccore/gateway/
+-rw-rw-rw-   0        0        0      220 2023-07-13 02:00:35.000000 asynccore-1.2.1/asynccore/gateway/__init__.py
+-rw-rw-rw-   0        0        0      662 2023-07-02 18:23:21.000000 asynccore-1.2.1/asynccore/gateway/enums.py
+-rw-rw-rw-   0        0        0      845 2023-07-13 02:08:33.000000 asynccore-1.2.1/asynccore/gateway/errors.py
+-rw-rw-rw-   0        0        0     5214 2023-07-13 02:08:32.000000 asynccore-1.2.1/asynccore/gateway/event.py
+-rw-rw-rw-   0        0        0    15248 2023-07-13 02:38:54.000000 asynccore-1.2.1/asynccore/gateway/gateway.py
+-rw-rw-rw-   0        0        0     2044 2023-07-13 02:08:32.000000 asynccore-1.2.1/asynccore/gateway/response.py
+-rw-rw-rw-   0        0        0    10552 2023-07-13 02:30:50.000000 asynccore-1.2.1/asynccore/http.py
+-rw-rw-rw-   0        0        0      866 2023-07-13 02:08:32.000000 asynccore-1.2.1/asynccore/logger.py
+-rw-rw-rw-   0        0        0      591 2023-07-13 02:08:32.000000 asynccore-1.2.1/asynccore/permissionbuilder.py
+-rw-rw-rw-   0        0        0     2753 2023-07-13 02:00:35.000000 asynccore-1.2.1/asynccore/tasks.py
+-rw-rw-rw-   0        0        0      463 2023-07-13 02:26:51.000000 asynccore-1.2.1/asynccore/typings.py
+-rw-rw-rw-   0        0        0    34586 2023-07-13 02:37:48.000000 asynccore-1.2.1/asynccore/user.py
+drwxrwxrwx   0        0        0        0 2023-07-21 10:40:13.826489 asynccore-1.2.1/asynccore.egg-info/
+-rw-rw-rw-   0        0        0     2786 2023-07-21 10:40:13.000000 asynccore-1.2.1/asynccore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      772 2023-07-21 10:40:13.000000 asynccore-1.2.1/asynccore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 10:40:13.000000 asynccore-1.2.1/asynccore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-07-21 10:40:13.000000 asynccore-1.2.1/asynccore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-21 10:40:13.000000 asynccore-1.2.1/asynccore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      730 2023-07-13 02:41:16.000000 asynccore-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-21 10:40:13.832469 asynccore-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1311 2023-07-21 10:30:13.000000 asynccore-1.2.1/setup.py
```

### Comparing `asynccore-1.2.0/PKG-INFO` & `asynccore-1.2.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-Metadata-Version: 2.1
-Name: asynccore
-Version: 1.2.0
-Summary: Library that will allow you to manage selfbots
-Author: xXenvy
-Author-email: <xpimpek01@gmail.com>
-Keywords: python,requests,discord selfbot,selfbot,discord.py,aiohttp
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-
-
-**Project only for educational purposes! 🤓**
-
-[![Downloads](https://static.pepy.tech/personalized-badge/selfbotclient?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/selfbotclient)
-[![Documentation Status](https://readthedocs.org/projects/selfbotclient/badge/?version=latest)](https://selfbotclient.readthedocs.io/en/latest/?badge=latest)
-![master](https://img.shields.io/github/last-commit/badges/shields/master)
-![commits](https://badgen.net/github/commits/xXenvy/selfbotclient/master)
-
-## 🌐 Docs
-https://selfbotclient.readthedocs.io/en/latest/
-
-# ⚡ Fast Self Bot Client
-- Token Checker | `1` token / `140`ms
-- +10 requests / 1s `(using tasks)`
-
-https://github.com/xXenvy/SelfBotClient/assets/111158232/ede9fb47-d489-4d9a-b58d-95c06dea6fe9
-
-
-# 🔧 Full control
-- A separate method to send your own requests
-- Ability to manage individual selfbots
-
-# 📌 Ratelimit handler
-- The library itself detects whether you have reached the ratelimit of the discord and, if so, forces you to wait a certain time.
-![Test](https://i.imgur.com/hTUFQKF.png)
-# 🛠️ Installation
-```shell
-pip install -U asynccore
-```
-# 💫 Usage
-
-```py
-from asynccore import Client
-
-tokens: list[str] = ["TOKEN_1", "TOKEN_2"]
-
-client: Client = Client(api_version=10)
-client.login(token=tokens)
-```
-**See more examples on github:** [Examples](https://github.com/xXenvy/SelfBotClient/tree/master/examples)
+### The most powerful discord selfbotting library.
+> ⚠️ Project only for educational purposes! 🤓
+> 
+![License](https://img.shields.io/github/license/xXenvy/AsyncCore?style=for-the-badge&color=%2315b328)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/AsyncCore?style=for-the-badge&color=%2315b328)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/t/xXenvy/AsyncCore?style=for-the-badge&color=%2315b328)
+![GitHub last commit (branch)](https://img.shields.io/github/last-commit/xXenvy/AsyncCore/master?style=for-the-badge&color=%2315b328)
+
+# 💢 Requirements
+> Python 3.9 or newer
+
+# 🔧 AsyncCore Features
+- Modern Pythonic API using `async` and `await`
+- Proper rate limit handling
+- Optimised in both `speed` and `memory`
+- Properly typehinted
+
+## ⚡ High Speed
+https://github.com/xXenvy/SelfBotClient/assets/111158232/ede9fb47-d489-4d9a-b58d-95c06dea6fe9
+
+## 🔧 Full control
+- A separate method to send your own requests
+- Ability to manage individual selfbots
+- Simple multi-account management
+
+## 📌 Ratelimit handler
+- The library itself detects whether you have reached the ratelimit of the discord and, if so, forces you to wait a certain time.
+![Test](https://i.imgur.com/hTUFQKF.png)
+
+# 🛠️ Installation
+```shell
+pip install -U asynccore
+```
+# 💫 Example
+**See more examples on github:** [JUMP!](https://github.com/xXenvy/SelfBotClient/tree/master/examples)
+```py
+from asynccore import Client, UserClient
+
+client: Client = Client(api_version=10)
+client.login(tokens=["TOKEN_1", "TOKEN_2"])
+
+async def send_example_message(user: UserClient, channel_id: int) -> None:
+    await user.send_message(channel_id=channel_id, message_content="Hi")
+
+@client.gateway.event(event_name="on_ready")
+async def ready(user: UserClient):
+    print(f"Account: {user.name} is ready.")
+    await send_example_message(user=user, channel_id=123)
+
+client.gateway.run(reconnect=True)
+```
+
+# 🧷 Links
+- [Documentation](https://asynccore.readthedocs.io/en/latest/index.html)
+- [Report a bug or feature](https://github.com/xXenvy/AsyncCore/issues/new/choose)
```

### Comparing `asynccore-1.2.0/asynccore/__init__.py` & `asynccore-1.2.1/asynccore/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 from .client import Client
-from .enums import ChannelType, Permissions, ActivityType, ActivityPlatform, ActivityStatus
-from .typings import ClientResponse, RGB_COLOR
+from .enums import (
+    ChannelType,
+    Permissions,
+    ActivityType,
+    ActivityPlatform,
+    ActivityStatus,
+)
+from .typings import RGB_COLOR, ClientResponse
 from .permissionbuilder import PermissionBuilder
 from .activity import ActivityBuilder
 from .user import UserClient
 
 
 __all__: tuple[str, ...] = (
     "Client",
@@ -13,9 +19,9 @@
     "RGB_COLOR",
     "Permissions",
     "PermissionBuilder",
     "UserClient",
     "ActivityType",
     "ActivityStatus",
     "ActivityPlatform",
-    "ActivityBuilder"
+    "ActivityBuilder",
 )
```

### Comparing `asynccore-1.2.0/asynccore/activity.py` & `asynccore-1.2.1/asynccore/activity.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,21 +13,22 @@
     :param activity_name: Set the name of the activity
     :param activity_type: Set the activity type
     :param activity_details: Display the name of the game you are playing
     :param user_status: Set the user status
     :param user_platform: Set the platform that the user is using
     """
 
-    def __init__(self,
-                 activity_name: str,
-                 activity_type: ActivityType,
-                 activity_details: str = "",
-                 user_status: ActivityStatus = ActivityStatus.ONLINE,
-                 user_platform: ActivityPlatform = ActivityPlatform.DESKTOP,
-                 ):
+    def __init__(
+        self,
+        activity_name: str,
+        activity_type: ActivityType,
+        activity_details: str = "",
+        user_status: ActivityStatus = ActivityStatus.ONLINE,
+        user_platform: ActivityPlatform = ActivityPlatform.DESKTOP,
+    ):
         self.activity_name: str = activity_name
         self.activity_details: str = activity_details
 
         if isinstance(activity_type, ActivityType):
             self.activity_type: int = activity_type.value
         else:
             raise InvalidStatusType(ActivityType, type(activity_type))
```

### Comparing `asynccore-1.2.0/asynccore/cache.py` & `asynccore-1.2.1/asynccore/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import TYPE_CHECKING, Optional, Any
 
 from .typings import AUTH_HEADER
 
 if TYPE_CHECKING:
     from .client import ClientResponse, UserClient
     from .http import CustomSession
-    from .user import UserClient
     from .gateway.response import GatewayResponse
 
 
 class Cache:
     """
     A Cache object is assigned to each :class:`asynccore.user.UserClient` object. It stores servers, channels, messages.
     The startup function acquires all data (except messages) at startup if **startup_cache**
@@ -35,17 +34,15 @@
         self.__cached_channels: dict[guild_id, list[dict[str, Any]]] = {}
         self.__cached_messages: dict[guild_id, list[dict[str, Any]]] = {}
 
     async def __request_guilds(self):
         url: str = self._endpoint + "users/@me/guilds"
 
         response: ClientResponse = await self.session.request(
-            url=url,
-            method="GET",
-            headers=AUTH_HEADER(authorization=self.user.token)
+            url=url, method="GET", headers=AUTH_HEADER(authorization=self.user.token)
         )
 
         if response.status == 200:
             guilds_data = await response.json()
             for guild in guilds_data:
                 if guild["id"] not in self.__cached_guilds:
                     self.__cached_guilds.append(guild)
@@ -55,19 +52,22 @@
             guild_id: int = int(guild_data["id"])
 
             url: str = self._endpoint + f"guilds/{guild_id}/channels"
 
             response: ClientResponse = await self.session.request(
                 url=url,
                 method="GET",
-                headers=AUTH_HEADER(authorization=self.user.token)
+                headers=AUTH_HEADER(authorization=self.user.token),
             )
 
             if response.status == 200:
-                if guild_id not in self.__cached_channels.keys():  # pylint: disable=consider-iterating-dictionary
+                if (
+                    guild_id
+                    not in self.__cached_channels.keys()  # pylint: disable=consider-iterating-dictionary
+                ):
                     channels_data: list[dict] = await response.json()
                     self.__cached_channels[guild_id] = channels_data
 
     async def __request_messages(self):  # pylint: disable=unused-private-member
         ...
 
         # Disabled due to long startup time and ratelimit
@@ -102,15 +102,17 @@
             in the :class:`asynccore.client.Client` class.
         """
 
         if not self.__cached_guilds:
             await self.__request_guilds()
             await self.__request_channels()
 
-    def get_channel(self, channel_id: int, guild_id: Optional[int] = None) -> Optional[dict]:
+    def get_channel(
+        self, channel_id: int, guild_id: Optional[int] = None
+    ) -> Optional[dict]:
         """
         The get_channel function is used to retrieve a channel's data from the cache.
 
         :param channel_id: Get the channel id of a specific channel
         :param guild_id: Specify the guild id of the channel
         """
 
@@ -191,21 +193,23 @@
         :param guild_id: Specify the guild id of the message
         :param message_id: Find the message in the list of messages
         """
 
         messages: Optional[list[dict]] = self.__cached_messages.get(int(guild_id))
 
         if not messages:
-            return
+            return None
 
         for message in messages:
             if int(message["id"]) == int(message_id):
                 return message
 
-    def get_messages_from_channel(self, guild_id: int, channel_id: int) -> Optional[list[Optional[dict]]]:
+    def get_messages_from_channel(
+        self, guild_id: int, channel_id: int
+    ) -> Optional[list[Optional[dict]]]:
         """
         The get_messages_from_channel function takes a guild_id and channel_id,
         and returns all messages from the specified channel. If no messages are found,
         it will return None.
 
         :param guild_id: Get the messages from a specific guild
         :param channel_id: Get the messages from a specific channel
@@ -229,31 +233,38 @@
     def add_channel_to_cache(self, channel_data: dict) -> None:
         """
         The add_channel_to_cache function adds a channel to the cache.
 
         :param channel_data: Pass the channel data
         """
 
-        guild_id: int = int(channel_data["guild_id"])
+        guild_id: Optional[int] = channel_data.get("guild_id")
+        if not guild_id:
+            return
 
+        guild_id = int(guild_id)
         if self.__cached_channels.get(guild_id):
             cached_channels: list = self.__cached_channels[guild_id]
             cached_channels.append(channel_data)
             self.__cached_channels[guild_id] = cached_channels
         else:
             self.__cached_channels[guild_id] = [channel_data]
 
     def add_message_to_cache(self, message_data: dict) -> None:
         """
         The add_message_to_cache function adds a message to the cache.
 
         :param message_data: Pass in the message data that is to be added to the cache
         """
 
-        guild_id: int = int(message_data["guild_id"])
+        guild_id: Optional[int] = message_data.get("guild_id")
+        if not guild_id:
+            return
+
+        guild_id = int(guild_id)
 
         if self.__cached_messages.get(guild_id):
             cached_messages: list = self.__cached_messages[guild_id]
             cached_messages.append(message_data)
             self.__cached_messages[guild_id] = cached_messages
         else:
             self.__cached_messages[guild_id] = [message_data]
@@ -323,17 +334,17 @@
         :param guild_data: Pass in the guild data
         """
 
         guild_id: int = int(guild_data["id"])
 
         guilds: Optional[list[dict]] = self.__cached_guilds
 
-        if not len(guilds):
+        if not guilds:
             self.__cached_guilds = [guild_data]
-            return
+            return None
 
         for index, guild in enumerate(guilds):
             if int(guild["id"]) == guild_id:
                 del guilds[index]
 
         guilds.append(guild_data)
         self.__cached_messages[guild_id] = guilds
@@ -373,27 +384,31 @@
 
         args: Optional[tuple] = None
 
         if self.event_name == "MESSAGE_UPDATE":
             guild_id: int = int(self.response.data["guild_id"])
             message_id: int = int(self.response.data["id"])
 
-            before_message: Optional[dict] = self.user.cache.get_message(guild_id, message_id)
+            before_message: Optional[dict] = self.user.cache.get_message(
+                guild_id, message_id
+            )
 
             if not before_message:
                 before_message = {}
 
             args = (self.user, before_message, self.response.data)
 
             self.user.cache.update_message(guild_id, self.response.data)
 
         if self.event_name == "CHANNEL_UPDATE":
             guild_id: int = int(self.response.data["guild_id"])
             channel_id: int = int(self.response.data["id"])
-            before_channel: Optional[dict] = self.user.cache.get_channel(channel_id, guild_id)
+            before_channel: Optional[dict] = self.user.cache.get_channel(
+                channel_id, guild_id
+            )
 
             if not before_channel:
                 before_channel = {}
 
             args = (self.user, before_channel, self.response.data)
 
             self.user.cache.update_channel(guild_id, self.response.data)
```

### Comparing `asynccore-1.2.0/asynccore/client.py` & `asynccore-1.2.1/asynccore/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,30 +25,37 @@
     :param request_latency: Control the rate of requests sent to discord
     :param ratelimit_additional_cooldown: Add a cooldown to the ratelimit
     :param use_tasks: Enable or disable the tasks option (:class:`asynccore.tasks`), which for now is in beta.
     :param activity: The argument with type :class:`AcivityBuilder` is responsible for account activity.
     :param startup_cache: Enable or disable cache fetching at program startup
     """
 
-    __version__: str = "1.2.0"
+    __version__: str = "1.2.1"
 
     def __init__(
-            self,
-            api_version: API_VERSION,
-            loop: Union[AbstractEventLoop, None] = None,
-            logger: bool = True,
-            request_latency: float = 0.1,
-            ratelimit_additional_cooldown: float = 10,
-            use_tasks: bool = False,
-            activity: Optional[ActivityBuilder] = None,
-            startup_cache: bool = False
+        self,
+        api_version: API_VERSION,
+        loop: Union[AbstractEventLoop, None] = None,
+        logger: bool = True,
+        request_latency: float = 0.1,
+        ratelimit_additional_cooldown: float = 10,
+        use_tasks: bool = False,
+        activity: Optional[ActivityBuilder] = None,
+        startup_cache: bool = False,
     ):  # type: ignore
-
-        super().__init__(api_version, loop, logger, request_latency,
-                         ratelimit_additional_cooldown, self, activity, startup_cache)
+        super().__init__(
+            api_version,
+            loop,
+            logger,
+            request_latency,
+            ratelimit_additional_cooldown,
+            self,
+            activity,
+            startup_cache,
+        )
 
         if use_tasks:
             self.tasks: Tasks = Tasks(client=self)
 
     def login(self, tokens: Union[str, list[str]]) -> None:
         """
         The login function is used to check the provided tokens.
@@ -57,82 +64,101 @@
         """
 
         if self.logger._status:  # pyright: ignore
             self.logger.info("Checking the provided tokens")
 
         self._check_tokens(tokens)
 
-    async def send_message(self, channel_id: int, message_content: str) -> Optional[AsyncIterable[ClientResponse]]:
+    async def send_message(
+        self, channel_id: int, message_content: str
+    ) -> Optional[AsyncIterable[ClientResponse]]:
         """
         The send_message function sends a message to the specified channel.
 
         :param channel_id: Specify the channel to send the message to
         :param message_content: content of the message
         """
 
         for user in self.users:
-            response: ClientResponse = await user.send_message(channel_id, message_content)
+            response: ClientResponse = await user.send_message(
+                channel_id, message_content
+            )
             yield response
 
-    async def reply_message(self, channel_id: int, message_id: int,
-                            message_content: str, mention_author: bool = True) -> Union[
-        None, AsyncIterable[ClientResponse]]:
-
+    async def reply_message(
+        self,
+        channel_id: int,
+        message_id: int,
+        message_content: str,
+        mention_author: bool = True,
+    ) -> Union[None, AsyncIterable[ClientResponse]]:
         """
         The reply_message function is used to reply to a message in a channel.
 
         :param channel_id: Specify the channel to send the message in
         :param message_id: Reply to a specific message
         :param message_content: Message content
         :param mention_author: Determine whether or not the author of the message should be mentioned in
         """
 
         for user in self.users:
-            response: ClientResponse = await user.reply_message(channel_id, message_id, message_content, mention_author)
+            response: ClientResponse = await user.reply_message(
+                channel_id, message_id, message_content, mention_author
+            )
             yield response
 
-    async def edit_message(self, channel_id: int, message_id: int, message_content: str) -> Optional[ClientResponse]:
+    async def edit_message(
+        self, channel_id: int, message_id: int, message_content: str
+    ) -> Optional[ClientResponse]:
         """
         The edit_message function allows you to edit a message.
 
         :param channel_id: Specify the channel id of the message you want to edit
         :param message_id: id the message to edit
         :param message_content: Edit the message content
         """
 
         for user in self.users:
-            response: ClientResponse = await user.edit_message(channel_id, message_id, message_content)
+            response: ClientResponse = await user.edit_message(
+                channel_id, message_id, message_content
+            )
             if response.status == 200:
                 return response
 
-    async def get_message(self, channel_id: int, message_id: int) -> Optional[AsyncIterable[ClientResponse]]:
+    async def get_message(
+        self, channel_id: int, message_id: int
+    ) -> Optional[AsyncIterable[ClientResponse]]:
         """
         The get_message function is used to get a message from a channel.
 
         :param channel_id: Specify the channel id of the message you want to get
         :param message_id: Get the message around that id
         """
         for user in self.users:
             response: ClientResponse = await user.get_message(channel_id, message_id)
             yield response
 
-    async def get_messages(self, channel_id: int, limit: int = 100) -> Optional[ClientResponse]:
+    async def get_messages(
+        self, channel_id: int, limit: int = 100
+    ) -> Optional[ClientResponse]:
         """
         The get_messages function is used to retrieve a list of message objects from the channel.
 
         :param channel_id: Specify which channel to get the messages from
         :param limit: Limit the number of messages returned
         """
 
         for user in self.users:
             response: ClientResponse = await user.get_messages(channel_id, limit)
             if response.status == 200:
                 return response
 
-    async def delete_message(self, channel_id: int, message_id: int) -> Optional[ClientResponse]:
+    async def delete_message(
+        self, channel_id: int, message_id: int
+    ) -> Optional[ClientResponse]:
         """
         The delete_message function deletes a message from the specified channel.
 
         :param channel_id: Specify the channel id of the message to be deleted
         :param message_id: Identify the message that is to be deleted
         """
         for user in self.users:
@@ -148,15 +174,17 @@
         """
 
         for user in self.users:
             response: ClientResponse = await user.delete_channel(channel_id)
             if response.status == 200:
                 return response
 
-    async def delete_channels(self, channel_ids: list[int]) -> Optional[AsyncIterable[ClientResponse]]:
+    async def delete_channels(
+        self, channel_ids: list[int]
+    ) -> Optional[AsyncIterable[ClientResponse]]:
         """
         The delete_channels function takes a list of channel_ids and deletes them.
 
         It returns an AsyncIterable of ClientResponse objects,
         which can be used to check the status code for each request.
 
         :param channel_ids: Specify the list of channel ids that will be deleted
@@ -164,36 +192,45 @@
 
         while len(channel_ids):
             for user in self.users:
                 channel_id: int = channel_ids.pop(0)
                 response: ClientResponse = await user.delete_channel(channel_id)
                 yield response
 
-    async def create_channel(self, guild_id: int, name: str, channel_type: ChannelType,
-                             topic: Optional[str] = None, user_limit: Optional[int] = None,
-                             position: Optional[int] = None, nsfw: Optional[bool] = False) -> Optional[
-        AsyncIterable[ClientResponse]]:
+    async def create_channel(
+        self,
+        guild_id: int,
+        name: str,
+        channel_type: ChannelType,
+        topic: Optional[str] = None,
+        user_limit: Optional[int] = None,
+        position: Optional[int] = None,
+        nsfw: Optional[bool] = False,
+    ) -> Optional[AsyncIterable[ClientResponse]]:
         """
         The create_channel function creates a channel in the specified guild.
 
         :param guild_id: Specify the guild id of the server you want to create a channel in
         :param name: Specify the name of the channel
         :param channel_type: Specify what type of channel you want to create
         :param topic: Set the topic of the channel
         :param user_limit: Set the maximum number of users allowed in a voice channel
         :param position: Set the position of the channel in the list
         :param nsfw: Determine whether the channel is nsfw or not
         """
 
         for user in self.users:
-            response: ClientResponse = await user.create_channel(guild_id, name, channel_type, topic, user_limit,
-                                                                 position, nsfw)
+            response: ClientResponse = await user.create_channel(
+                guild_id, name, channel_type, topic, user_limit, position, nsfw
+            )
             yield response
 
-    async def get_channels(self, guild_id: int) -> Optional[AsyncIterable[ClientResponse]]:
+    async def get_channels(
+        self, guild_id: int
+    ) -> Optional[AsyncIterable[ClientResponse]]:
         """
         The get_channels function is a coroutine that takes in a guild_id
         and returns an AsyncIterable of ClientResponse objects.
 
         The function can return the data of all channels on the server
 
         :param guild_id: Specify the guild id of the server you want to get channels from
@@ -211,60 +248,69 @@
         """
 
         for user in self.users:
             response: ClientResponse = await user.get_channel(channel_id)
             if response.status == 200:
                 return response
 
-    async def create_role(self, guild_id: int,
-                          name: str,
-                          color: Optional[RGB_COLOR] = None,
-                          hoist: Optional[bool] = False,
-                          permissions: Optional[PermissionBuilder] = None) \
-            -> Optional[AsyncIterable[ClientResponse]]:
+    async def create_role(
+        self,
+        guild_id: int,
+        name: str,
+        color: Optional[RGB_COLOR] = None,
+        hoist: Optional[bool] = False,
+        permissions: Optional[PermissionBuilder] = None,
+    ) -> Optional[AsyncIterable[ClientResponse]]:
         """
         The create_role function creates a role in the specified guild.
 
         :param guild_id: Specify the guild in which you want to create a role
         :param name: Set the name of the role
         :param color: Set the color of the role
         :param hoist: Determine whether the role should be displayed separately in the user list
         :param permissions: Set the permissions for the role
         """
 
         for user in self.users:
-            response: ClientResponse = await user.create_role(guild_id, name, color, hoist, permissions)
+            response: ClientResponse = await user.create_role(
+                guild_id, name, color, hoist, permissions
+            )
             yield response
 
-    async def get_roles(self, guild_id: int) -> Union[None, AsyncIterable[ClientResponse]]:
+    async def get_roles(
+        self, guild_id: int
+    ) -> Union[None, AsyncIterable[ClientResponse]]:
         """
         get_roles returns a list of data with all the roles on the server
 
         :param guild_id: Specify the guild id of the server you want to get roles from
         """
         for user in self.users:
             response: ClientResponse = await user.get_roles(guild_id)
             yield response
 
-    async def delete_roles(self, guild_id: int, role_ids: list[int]) -> Union[None, AsyncIterable[ClientResponse]]:
-
+    async def delete_roles(
+        self, guild_id: int, role_ids: list[int]
+    ) -> Union[None, AsyncIterable[ClientResponse]]:
         """
         delete_roles function removes all roles with id in the list
 
         :param guild_id: Specify the guild that the roles are being deleted from
         :param role_ids: Specify the roles that are to be deleted
         """
 
         while len(role_ids):
             for user in self.users:
                 role_id: int = role_ids.pop(0)
                 response: ClientResponse = await user.delete_role(guild_id, role_id)
                 yield response
 
-    async def delete_role(self, guild_id: int, role_id: int) -> Union[None, ClientResponse]:
+    async def delete_role(
+        self, guild_id: int, role_id: int
+    ) -> Union[None, ClientResponse]:
         """
         The delete_role function deletes a role from the guild.
 
         :param guild_id: int: Specify the guild that you want to delete a role from
         :param role_id: int: Specify the role_id to be deleted
         """
 
@@ -281,28 +327,32 @@
         """
 
         for user in self.users:
             response: ClientResponse = await user.get_guild_bans(guild_id)
             if response.status == 200:
                 return response
 
-    async def ban_member(self, guild_id: int, user_id: int) -> Union[None, ClientResponse]:
+    async def ban_member(
+        self, guild_id: int, user_id: int
+    ) -> Union[None, ClientResponse]:
         """
         The ban_member function is used to ban a member from the guild.
 
         :param guild_id: Specify the guild that you want to ban a user from
         :param user_id: Specify the user that is to be banned
         """
 
         for user in self.users:
             response: ClientResponse = await user.ban_member(guild_id, user_id)
             if response.status == 204:
                 return response
 
-    async def unban_members(self, guild_id: int, user_ids: list[int]) -> Union[None, AsyncIterable[ClientResponse]]:
+    async def unban_members(
+        self, guild_id: int, user_ids: list[int]
+    ) -> Union[None, AsyncIterable[ClientResponse]]:
         """
         The unban_members function is a coroutine that takes in a guild_id and user_ids list.
         It then iterates through the users list, popping off the first user id from the
         user_ids list and passing it to unban_member function of each client. If there is no
         response or if there was an error, it will return None. Otherwise, it will yield back
         the response.
 
@@ -313,29 +363,32 @@
         while len(user_ids):
             for user in self.users:
                 user_id: int = user_ids.pop(0)
                 response: ClientResponse = await user.unban_member(guild_id, user_id)
                 if response.status == 204:
                     yield response
 
-    async def unban_member(self, guild_id: int, user_id: int) -> Union[None, ClientResponse]:
+    async def unban_member(
+        self, guild_id: int, user_id: int
+    ) -> Union[None, ClientResponse]:
         """
         The unban_member function unban a user from the guild.
 
         :param guild_id: Specify the guild that you want to unban a member from
         :param user_id: Specify the user id of the member to unban
         """
 
         for user in self.users:
             response: ClientResponse = await user.unban_member(guild_id, user_id)
             if response.status == 204:
                 return response
 
-    async def ban_members(self, guild_id: int, user_ids: list[int]) -> Union[None, AsyncIterable[ClientResponse]]:
-
+    async def ban_members(
+        self, guild_id: int, user_ids: list[int]
+    ) -> Union[None, AsyncIterable[ClientResponse]]:
         """
         The ban_members function is a coroutine that takes in a guild_id and user_ids list.
         It then iterates through the users list, popping off the first user id from the
         user_ids list and passing it to ban_member function of each client. The response
         from each client is yielded back to whatever called this function.
 
         :param guild_id: Specify the guild to ban the user from
@@ -344,27 +397,31 @@
 
         while len(user_ids):
             for user in self.users:
                 user_id: int = user_ids.pop(0)
                 response: ClientResponse = await user.ban_member(guild_id, user_id)
                 yield response
 
-    async def kick_member(self, guild_id: int, user_id: int) -> Union[None, ClientResponse]:
+    async def kick_member(
+        self, guild_id: int, user_id: int
+    ) -> Union[None, ClientResponse]:
         """
         The kick_member function kicks a member from the guild.
 
         :param guild_id: Specify the guild that you want to kick a user from
         :param user_id: Identify the user to be kicked
         """
         for user in self.users:
             response: ClientResponse = await user.kick_member(guild_id, user_id)
             if response.status == 204:
                 return response
 
-    async def kick_members(self, guild_id: int, user_ids: list[int]) -> Union[None, AsyncIterable[ClientResponse]]:
+    async def kick_members(
+        self, guild_id: int, user_ids: list[int]
+    ) -> Union[None, AsyncIterable[ClientResponse]]:
         """
         The kick_members function is a coroutine that takes in a guild_id and user_ids list.
         It then iterates through the users list, popping off the first user id from the
         user_ids list and kicking them from the specified guild. It yields each response as it goes.
 
         :param guild_id: Specify which guild the user is in
         :param user_ids: list with id of people to kick out
@@ -372,94 +429,113 @@
 
         while len(user_ids):
             for user in self.users:
                 user_id: int = user_ids.pop(0)
                 response: ClientResponse = await user.kick_member(guild_id, user_id)
                 yield response
 
-    async def get_member(self, guild_id: int, user_id: int) -> Union[None, ClientResponse]:
+    async def get_member(
+        self, guild_id: int, user_id: int
+    ) -> Union[None, ClientResponse]:
         """
         The get_member function is used to get a member from the guild.
 
         :param guild_id: Specify the guild that you want to get a member from
         :param user_id: Specify the user id of the member you want to get
         """
 
         for user in self.users:
             response: ClientResponse = await user.get_member(guild_id, user_id)
             if response.status == 200:
                 return response
 
-    async def edit_member(self, guild_id: int, user_id: int,
-                          nickname: Optional[str] = None,
-                          add_roles: Optional[list[int]] = None,
-                          remove_roles: Optional[list[int]] = None) -> Union[None, ClientResponse]:
-
+    async def edit_member(
+        self,
+        guild_id: int,
+        user_id: int,
+        nickname: Optional[str] = None,
+        add_roles: Optional[list[int]] = None,
+        remove_roles: Optional[list[int]] = None,
+    ) -> Union[None, ClientResponse]:
         """
         The edit_member function allows you to edit a member of a guild.
 
         :param guild_id: Specify the guild that you want to edit a member in
         :param user_id: Specify the user that you want to edit
         :param nickname: Change the nickname of a user in a guild
         :param add_roles: Add roles to a user
         :param remove_roles: Remove roles from a user
         """
 
         for user in self.users:
-            response: ClientResponse = await user.edit_member(guild_id, user_id, nickname, add_roles, remove_roles)
+            response: ClientResponse = await user.edit_member(
+                guild_id, user_id, nickname, add_roles, remove_roles
+            )
             if response and response.status == 200:
                 return response
 
-    async def add_reaction(self, channel_id: int, message_id: int, emoji: str) \
-            -> Union[None, AsyncIterable[ClientResponse]]:
+    async def add_reaction(
+        self, channel_id: int, message_id: int, emoji: str
+    ) -> Union[None, AsyncIterable[ClientResponse]]:
         """
         The add_reaction function adds a reaction to the message with the given ID in the channel with
         the given ID. The emoji parameter is a string that must be an emoticon. Example: \N{FIRE}
 
         :param channel_id: Specify which channel_id the message is in
         :param message_id: Message ID that you want to add a reaction to
         :param emoji: A reaction to add to the message
         """
 
         for user in self.users:
-            response: ClientResponse = await user.add_reaction(channel_id, message_id, emoji)
+            response: ClientResponse = await user.add_reaction(
+                channel_id, message_id, emoji
+            )
             yield response
 
-    async def get_reactions(self, channel_id: int, message_id: int, emoji: str) -> Union[None, ClientResponse]:
+    async def get_reactions(
+        self, channel_id: int, message_id: int, emoji: str
+    ) -> Union[None, ClientResponse]:
         """
         The get_reactions function returns a ClientResponse with
         list of users that reacted with the specified emoji.
 
         :param channel_id: Identify the channel that contains the message
         :param message_id: Identify the message that is being reacted to
         :param emoji: Specify the emoji to get reactions for
         """
 
         for user in self.users:
-            response: ClientResponse = await user.get_reactions(channel_id, message_id, emoji)
+            response: ClientResponse = await user.get_reactions(
+                channel_id, message_id, emoji
+            )
             if response.status == 204:
                 return response
 
-    async def delete_reaction(self, channel_id: int, message_id: int, user_id: int, emoji: str) \
-            -> Union[None, ClientResponse]:
+    async def delete_reaction(
+        self, channel_id: int, message_id: int, user_id: int, emoji: str
+    ) -> Union[None, ClientResponse]:
         """
         The delete_reaction function is used to delete a reaction from a message.
 
         :param channel_id: Specify the channel where the message is located
         :param message_id: Identify the message that you want to delete a reaction from
         :param user_id: Specify the user whose reaction is to be deleted
         :param emoji: Specify the emoji to be deleted
         """
 
         for user in self.users:
-            response: ClientResponse = await user.delete_reaction(channel_id, message_id, user_id, emoji)
+            response: ClientResponse = await user.delete_reaction(
+                channel_id, message_id, user_id, emoji
+            )
             if response.status == 204:
                 return response
 
-    async def get_guild_invites(self, guild_id: int) -> Union[None, AsyncIterable[ClientResponse]]:
+    async def get_guild_invites(
+        self, guild_id: int
+    ) -> Union[None, AsyncIterable[ClientResponse]]:
         """
         The get_guild_invites function returns a list of invite objects. Requires the 'MANAGE_GUILD' permission.
 
         :param guild_id: Get the invites for a specific guild
         """
         for user in self.users:
             response: ClientResponse = await user.get_guild_invites(guild_id)
@@ -472,55 +548,64 @@
         :param guild_id: Specify the id of the guild you want to get information about
         """
         for user in self.users:
             response: ClientResponse = await user.get_guild(guild_id)
             if response.status == 200:
                 return response
 
-    async def send_dm_message(self, user_id: int, message_content: str) \
-            -> Union[None, AsyncIterable[Union[ClientResponse, None]]]:
+    async def send_dm_message(
+        self, user_id: int, message_content: str
+    ) -> Union[None, AsyncIterable[Union[ClientResponse, None]]]:
         """
         The send_dm_message function sends a direct message to the user with the given user_id.
 
         :param user_id: Specify the user id of the person you want to send a message to
         :param message_content: Specify the message content
         """
 
         for user in self.users:
-            response: Optional[ClientResponse] = await user.send_dm_message(user_id, message_content)
+            response: Optional[ClientResponse] = await user.send_dm_message(
+                user_id, message_content
+            )
             yield response
 
     async def on_ready(self, user: UserClient) -> None:
         ...
 
     async def on_message_create(self, user: UserClient, message_data: dict) -> None:
         ...
 
     async def on_message_delete(self, user: UserClient, message_data: dict) -> None:
         ...
 
-    async def on_message_edit(self, user: UserClient, before_data: dict, after_data: dict) -> None:
+    async def on_message_edit(
+        self, user: UserClient, before_data: dict, after_data: dict
+    ) -> None:
         ...
 
     async def on_message_reaction_add(self, user: UserClient, data: dict) -> None:
         ...
 
     async def on_message_reaction_remove(self, user: UserClient, data: dict) -> None:
         ...
 
     async def on_channel_create(self, user: UserClient, created_channel: dict) -> None:
         ...
 
     async def on_channel_delete(self, user: UserClient, deleted_channel: dict) -> None:
         ...
 
-    async def on_channel_edit(self, user: UserClient, before_data: dict, after_data: dict) -> None:
+    async def on_channel_edit(
+        self, user: UserClient, before_data: dict, after_data: dict
+    ) -> None:
         ...
 
-    async def on_guild_update(self, user: UserClient, before_data: dict, after_data: dict) -> None:
+    async def on_guild_update(
+        self, user: UserClient, before_data: dict, after_data: dict
+    ) -> None:
         ...
 
     async def on_guild_role_create(self, user: UserClient, role_data: dict) -> None:
         ...
 
     async def on_guild_role_delete(self, user: UserClient, role_data: dict) -> None:
         ...
```

### Comparing `asynccore-1.2.0/asynccore/commands/application.py` & `asynccore-1.2.1/asynccore/commands/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     A class representing the discord Application
 
     :param client: Pass the client object to the class
     :param application_id: Identify the application
     """
 
     def __init__(self, client: Client, application_id: int):
-
         self.client: Client = client
         self.application_id: int = application_id
         self._commands: Optional[dict] = None
 
         self._cached_commands: list[Optional[SlashCommand]] = []
 
     def __repr__(self):
@@ -43,17 +42,17 @@
         if len(self._cached_commands) >= 1:
             for slash in self._cached_commands:
                 if slash.global_name == command_name:  # pyright: ignore
                     return slash
 
         return None
 
-    async def search_slash_command(self, user: UserClient, guild_id: int, query: str, limit: int = 3) \
-            -> Optional[list[SlashCommand]]:
-
+    async def search_slash_command(
+        self, user: UserClient, guild_id: int, query: str, limit: int = 3
+    ) -> Optional[list[SlashCommand]]:
         """
         The search_slash_command function searches for slash commands in a guild.
 
         :param user: Get the gateway connection of the user
         :param guild_id: Specify the guild id of the server you want to search for commands in
         :param query: Search for commands with the given name
         :param limit: Limit the number of results returned
@@ -65,23 +64,27 @@
             raise GatewayNotConnected(f"{user} does not have a gateway connection. ")
 
         op: int = 24  # Code for requesting slash commands
         nonce: str = str((int(time()) * 1000 - 1420070400000) * 4194304)
 
         data = {
             "op": op,
-            "d": {"guild_id": guild_id,
-                  "nonce": nonce,
-                  "type": 1,
-                  "application_id": self.application_id,
-                  "query": query,
-                  "limit": limit},
+            "d": {
+                "guild_id": guild_id,
+                "nonce": nonce,
+                "type": 1,
+                "application_id": self.application_id,
+                "query": query,
+                "limit": limit,
+            },
         }
 
-        await gateway.application_update_request(data, self._await_for_application_commands_update)
+        await gateway.application_update_request(
+            data, self._await_for_application_commands_update
+        )
         data: Optional[dict] = None
 
         for _ in range(5):  # awaiting to gateway change self._commands to commands data
             await sleep(1)
             if self._commands:
                 data = self._commands
                 self._commands = None
@@ -91,28 +94,36 @@
             return []
 
         application_commands: list[dict] = data["application_commands"]
         slash_commands: Optional[list[SlashCommand]] = []
 
         for command_data in application_commands:
             if int(command_data["application_id"]) == self.application_id:
+                # If the command is the right bot
+
                 command_options: Optional[list[dict]] = command_data.get("options")
 
                 if command_options and command_options[0].get("type") == 1:
-
                     for sub_command_data in command_data["options"]:
-
-                        sub_command_data["application_id"] = command_data["application_id"]
+                        sub_command_data["application_id"] = command_data[
+                            "application_id"
+                        ]
                         sub_command_data["version"] = command_data["version"]
                         sub_command_data["id"] = command_data["id"]
-                        sub_command_data["default_member_permissions"] = command_data["default_member_permissions"]
+                        sub_command_data["default_member_permissions"] = command_data[
+                            "default_member_permissions"
+                        ]
                         sub_command_data["nsfw"] = command_data["nsfw"]
-                        sub_command_data["dm_permission"] = command_data["dm_permission"]
+                        sub_command_data["dm_permission"] = command_data[
+                            "dm_permission"
+                        ]
                         sub_command_data["contexts"] = command_data["contexts"]
-                        sub_command_data["global_name"] = f"{command_data['name']} {sub_command_data['name']}"
+                        sub_command_data[
+                            "global_name"
+                        ] = f"{command_data['name']} {sub_command_data['name']}"
                         sub_command_data["sub_command"] = sub_command_data["name"]
                         sub_command_data["name"] = command_data["name"]
 
                         options: dict = {
                             "type": sub_command_data["type"],
                             "name": sub_command_data["sub_command"],
                         }
@@ -120,20 +131,24 @@
                         if sub_command_data.get("options"):
                             options["options"] = sub_command_data.get("options")
                         else:
                             options["options"] = []
 
                         sub_command_data["options"] = [options]
 
-                        sub_command = SlashCommand(command_data=sub_command_data, client=self.client)
+                        sub_command = SlashCommand(
+                            command_data=sub_command_data, client=self.client
+                        )
                         slash_commands.append(sub_command)
 
                 else:
                     command_data["global_name"] = command_data["name"]
-                    slash_commands.append(SlashCommand(command_data=command_data, client=self.client))
+                    slash_commands.append(
+                        SlashCommand(command_data=command_data, client=self.client)
+                    )
 
         for slash in slash_commands:
             if slash not in self._cached_commands:
                 self._cached_commands.append(slash)
 
         return slash_commands
```

### Comparing `asynccore-1.2.0/asynccore/commands/slashcommands.py` & `asynccore-1.2.1/asynccore/commands/slashcommands.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,27 +17,27 @@
     A class representing the SlashCommand of the Application.
 
     :param command_data: Store the command data
     :param client: Get the client object
     """
 
     def __init__(self, command_data: dict, client: Client):
-
         self.client: Client = client
         self.command_data: dict = command_data
         self.application_id: int = self.command_data["application_id"]
         self.command_name: str = self.command_data["name"]
 
         self.sub_command: Optional[str] = self.command_data.get("sub_command")
         self.global_name: str = self.command_data["global_name"]
 
     def __repr__(self):
         return f"<SlashCommand(name={self.global_name}, application_id={self.application_id})>"
 
-    def _format_slash_command(self, option: dict, inputs: dict, options: list) -> list:
+    @staticmethod
+    def _format_slash_command(option: dict, inputs: dict, options: list) -> list:
         """
         A function that formats the slashcommand data that must be given in the request
 
         :param option: Pass the option data to the function
         :param inputs: Store the input data for the command
         :param options: Store the data from each option
         """
@@ -46,55 +46,60 @@
             if key == "name":
                 for option_name, option_value in inputs.items():
                     if value == option_name:
                         _type: int = option["type"]
                         __option_data: dict = {
                             "type": _type,
                             "name": option_name,
-                            "value": option_value
+                            "value": option_value,
                         }
                         options.append(__option_data)
         return options
 
-    def _format_sub_command(self, command_type: int, option: dict, inputs: dict, options: list) -> list:
+    @staticmethod
+    def _format_sub_command(
+        command_type: int, option: dict, inputs: dict, options: list
+    ) -> list:
         """
         A function that formats the subcommand data that must be given in the request
 
         :param command_type: Determine what type of command is being used
         :param option: Pass the option data to the function
         :param inputs: Store the input data for the command
         :param options: Store the data from each option
         """
 
         option_inputs_list: list[Optional[dict]] = []
 
-        if len(option["options"]) >= 1:
+        if len(option["options"]) >= 1:  # pylint: disable=R1702
             for subcommand_option in option["options"]:
                 for key, value in subcommand_option.items():
                     if key == "name":
                         for input_name, input_value in inputs.items():
                             if value == input_name:
                                 _type: int = subcommand_option["type"]
                                 __option_data: dict = {
                                     "type": _type,
                                     "name": input_name,
-                                    "value": input_value
+                                    "value": input_value,
                                 }
                                 option_inputs_list.append(__option_data)
 
         option_data: dict = {
             "type": command_type,
             "name": option["name"],
-            "options": option_inputs_list
-                            }
+            "options": option_inputs_list,
+        }
         options.append(option_data)
 
         return options
 
-    async def _reformat_data(self, data: dict, nonce: str, inputs: Optional[dict[Any, Any]] = None) -> dict:
+    async def _reformat_data(
+        self, data: dict, nonce: str, inputs: Optional[dict[Any, Any]] = None
+    ) -> dict:
         """
         The reformat_data function is used to reformat the data that is sent to Discord's API.
         The function takes in a dictionary of data, a nonce string, and an optional inputs dictionary.
 
         :param data: command_data from __init__ method
         :param nonce: Generate a random string that is used to identify the command
         :param inputs: Pass in the inputs for the command
@@ -113,70 +118,85 @@
 
         command_type: int = data["type"]
         options: Optional[list[dict]] = data.get("options")
 
         if options:
             for option in options:
                 if option["type"] == 3:  # Normal command
-                    for data in self._format_slash_command(option, inputs, []):
-                        formatted_options.append(data)
+                    for command_data in self._format_slash_command(option, inputs, []):
+                        formatted_options.append(command_data)
 
                 elif option["type"] == 1:  # Command with subcommands
-                    for data in self._format_sub_command(command_type, option, inputs, []):
-                        formatted_options.append(data)
+                    for command_data in self._format_sub_command(
+                        command_type, option, inputs, []
+                    ):
+                        formatted_options.append(command_data)
 
         default_member_permissions = self.command_data["default_member_permissions"]
         nsfw: bool = self.command_data["nsfw"]
         command_description: str = self.command_data["description"]
         dm_permissions: bool = self.command_data["dm_permission"]
         contexts = self.command_data["contexts"]
 
         new_data["version"] = version
         new_data["id"] = command_id
         new_data["name"] = command_name
         new_data["type"] = command_type
         new_data["options"] = formatted_options
-        new_data["application_command"] = {"id": command_id, "application_id": self.application_id,
-                                           "version": version, "default_member_permissions": default_member_permissions,
-                                           "type": command_type, "nsfw": nsfw, "name": command_name,
-                                           "description": command_description, "dm_permissions": dm_permissions,
-                                           "contexts": contexts, "options": options, "attachments": [], "nonce": nonce}
+        new_data["application_command"] = {
+            "id": command_id,
+            "application_id": self.application_id,
+            "version": version,
+            "default_member_permissions": default_member_permissions,
+            "type": command_type,
+            "nsfw": nsfw,
+            "name": command_name,
+            "description": command_description,
+            "dm_permissions": dm_permissions,
+            "contexts": contexts,
+            "options": options,
+            "attachments": [],
+            "nonce": nonce,
+        }
 
         return new_data
 
-    async def use_slash_command(self, user: UserClient, guild_id: int, channel_id: int,
-                                                        inputs: Optional[dict[str, Any]] = None) \
-            -> Optional[ClientResponse]:
+    async def use_slash_command(
+        self,
+        user: UserClient,
+        guild_id: int,
+        channel_id: int,
+        inputs: Optional[dict[str, Any]] = None,
+    ) -> Optional[ClientResponse]:
         """
         The use_slash_command function is used to send a slash command to Discord.
 
         :param user: Send the request to discord
         :param guild_id: Specify the guild id of the server you want to use this command in
         :param channel_id: Specify the channel id of the channel where you want to send your command
         :param inputs: Pass in the inputs that is needed for the command to run
         """
 
         url: str = "interactions"
         nonce: str = str((int(time()) * 1000 - 1420070400000) * 4194304)
 
-        data = await self._reformat_data(data=self.command_data, nonce=nonce, inputs=inputs)
+        data = await self._reformat_data(
+            data=self.command_data, nonce=nonce, inputs=inputs
+        )
 
         session_id: str = "".join(choice(ascii_letters + digits) for _ in range(32))
 
         payload = {
             "type": 2,
             "application_id": self.application_id,
             "guild_id": guild_id,
             "channel_id": channel_id,
             "data": data,
             "nonce": nonce,
-            "session_id": session_id
+            "session_id": session_id,
         }
 
         header = AUTH_HEADER(authorization=user.token)
         response: ClientResponse = await self.client.request(
-            url=url,
-            method="POST",
-            data=payload,
-            headers=header  # pyright: ignore
+            url=url, method="POST", data=payload, headers=header  # pyright: ignore
         )
         return response
```

### Comparing `asynccore-1.2.0/asynccore/components.py` & `asynccore-1.2.1/asynccore/components.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,39 +10,41 @@
 from .typings import AUTH_HEADER
 
 if TYPE_CHECKING:
     from .client import Client
     from .user import UserClient
     from . import ClientResponse
 
-__all__: tuple[str, str, str] = (
-    "Button",
-    "MessageComponents",
-    "SelectMenu"
-)
+__all__: tuple[str, str, str] = ("Button", "MessageComponents", "SelectMenu")
 
 
 class SelectMenu:
-
     def __init__(self, data: dict, application_id: int):
         self._data: dict = data
 
         self.application_id: int = application_id
         self.type: int = self._data["type"]
         self.placeholder: str = self._data["placeholder"]
         self.custom_id: Optional[str] = self._data.get("custom_id")
         self.max_values: int = self._data["max_values"]
         self.min_values: int = self._data["min_values"]
 
         self.options: Optional[list[dict]] = self._data.get("options")
         # Options are only available for SelectMenu with type 3
 
-    async def use(self, client: Client, user: UserClient, channel_id: int, message_id: int,
-                  guild_id: int, message_flags: int, values: list[Union[str, int]]) -> Optional[ClientResponse]:
-
+    async def use(
+        self,
+        client: Client,
+        user: UserClient,
+        channel_id: int,
+        message_id: int,
+        guild_id: int,
+        message_flags: int,
+        values: list[Union[str, int]],
+    ) -> Optional[ClientResponse]:
         """
         Use this function to send values in SelectMenu
 
 
         :param client: Client to make the request to discord
         :param user: User to send SelectMenu
         :param channel_id: Specify the channel id of the message that triggered this interaction
@@ -58,41 +60,40 @@
         session_id: str = "".join(choice(ascii_letters + digits) for _ in range(32))
         nonce = str((int(time()) * 1000 - 1420070400000) * 4194304)
 
         data: dict = {
             "component_type": self.type,
             "custom_id": self.custom_id,
             "type": self.type,
-            "values": values
+            "values": values,
         }
 
         payload: dict = {
             "type": 3,
             "nonce": nonce,
             "guild_id": guild_id,
             "channel_id": channel_id,
             "message_flags": message_flags,
             "message_id": message_id,
             "application_id": self.application_id,
             "data": data,
-            "session_id": session_id
+            "session_id": session_id,
         }
 
         headers: dict = AUTH_HEADER(authorization=user.token)  # pyright: ignore
 
         response: ClientResponse = await client.request(
-            url="interactions",
-            method="POST",
-            data=payload,
-            headers=headers
+            url="interactions", method="POST", data=payload, headers=headers
         )
         return response
 
     def __repr__(self):
-        return f"<SelectMenu(placeholder={self.placeholder}, custom_id={self.custom_id})>"
+        return (
+            f"<SelectMenu(placeholder={self.placeholder}, custom_id={self.custom_id})>"
+        )
 
 
 class Button:
     """
     The Button class is responsible for interacting with the button
 
     :param data: Store the data of the button
@@ -101,16 +102,23 @@
     def __init__(self, data: dict, application_id: int):
         self._data: dict = data
 
         self.application_id: int = application_id
         self.label: Optional[str] = self._data.get("label")
         self.custom_id: Optional[str] = self._data.get("custom_id")
 
-    async def use(self, client: Client, user: UserClient, channel_id: int, message_id: int,
-                  guild_id: int, message_flags: int) -> Optional[ClientResponse]:
+    async def use(
+        self,
+        client: Client,
+        user: UserClient,
+        channel_id: int,
+        message_id: int,
+        guild_id: int,
+        message_flags: int,
+    ) -> Optional[ClientResponse]:
         """
         The use function allows you to press a button
 
         :param client: Client needed to send a request
         :param user: User who is supposed to send a request who presses the button
         :param channel_id: Specify the channel id of the message that contains the button
         :param message_id: Identify the message that contains the button
@@ -126,24 +134,21 @@
             "nonce": nonce,
             "guild_id": guild_id,
             "channel_id": channel_id,
             "message_flags": message_flags,
             "message_id": message_id,
             "application_id": self.application_id,
             "data": self._data,
-            "session_id": session_id
+            "session_id": session_id,
         }
 
         headers: dict = AUTH_HEADER(authorization=user.token)  # pyright: ignore
 
         response: ClientResponse = await client.request(
-            url="interactions",
-            method="POST",
-            data=payload,
-            headers=headers
+            url="interactions", method="POST", data=payload, headers=headers
         )
         return response
 
     def __repr__(self):
         return f"<Button(label={self.label}, custom_id={self.custom_id})>"
 
 
@@ -174,16 +179,24 @@
             raise ValueError("Missing message components")
 
         buttons: list[Optional[Button]] = []
 
         for component in self.components:
             for _comp_data in component["components"]:
                 if _comp_data["type"] == self.types.BUTTON.value:
-                    buttons.append(Button({"component_type": 2, "custom_id": _comp_data.get("custom_id"),
-                                           "label": _comp_data["label"]}, self.application_id))
+                    buttons.append(
+                        Button(
+                            {
+                                "component_type": 2,
+                                "custom_id": _comp_data.get("custom_id"),
+                                "label": _comp_data["label"],
+                            },
+                            self.application_id,
+                        )
+                    )
         return buttons
 
     def _find_selectmenus(self) -> list[Optional[SelectMenu]]:
         """
         The _find_buttons function is a helper function that finds all the select menus in a message.
         It returns a list of SelectMenu objects, which are defined in the SelectMenu class.
         """
@@ -206,10 +219,9 @@
         """
 
         buttons = self._find_buttons()
 
         return buttons
 
     def get_selectmenus(self) -> list[Optional[SelectMenu]]:
-
         menus = self._find_selectmenus()
         return menus
```

### Comparing `asynccore-1.2.0/asynccore/enums.py` & `asynccore-1.2.1/asynccore/enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 from enum import Enum
 
 
-__all__: tuple[str, ...] = ("ChannelType", "Permissions", "Discord",
-                            "ActivityPlatform", "ActivityStatus", "ActivityType")
+__all__: tuple[str, ...] = (
+    "ChannelType",
+    "Permissions",
+    "Discord",
+    "ActivityPlatform",
+    "ActivityStatus",
+    "ActivityType",
+    "Components",
+)
 
 
 class Discord(Enum):
     ENDPOINT = "https://discord.com/api/v{}/"
     ENDPONT_GATEWAY = "wss://gateway.discord.gg/?v={}&encoding=json"
 
 
@@ -32,15 +39,14 @@
     STREAMING = 1
     LISTENING = 2
     WATCHING = 3
     COMPETING = 5
 
 
 class ChannelType(Enum):
-
     TEXT_CHANNEL = 0
     VOICE_CHANNEL = 2
     CATEGORY_CHANNEL = 4
 
 
 class Permissions(Enum):
     CREATE_INSTANT_INVITE = 1 << 0
```

### Comparing `asynccore-1.2.0/asynccore/errors.py` & `asynccore-1.2.1/asynccore/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 __all__: tuple[str, ...] = (
     "UnSupportedApiVersion",
     "UnSupportedTokenType",
-    "InvalidMethodType"
+    "InvalidMethodType",
+    "InvalidStatusType",
+    "MessagesLimitException",
 )
 
 
 class SelfBotClientException(Exception):
     pass
 
 
 class UnSupportedApiVersion(SelfBotClientException):
-
     def __init__(self) -> None:
-        super().__init__(
-            "Invalid Api Version. Currently supported versions: 10, 9"
-        )
+        super().__init__("Invalid Api Version. Currently supported versions: 10, 9")
 
 
 class UnSupportedTokenType(SelfBotClientException):
-
     def __init__(self) -> None:
-        super().__init__(
-            "Invalid token/s type. Use list[str] or str."
-        )
+        super().__init__("Invalid token/s type. Use list[str] or str.")
 
 
 class InvalidMethodType(SelfBotClientException):
-
     def __init__(self, method: str) -> None:
         super().__init__(
             f"Invalid method {method} type. Available methods: POST, DELETE, GET, PATCH"
         )
 
 
 class InvalidStatusType(SelfBotClientException):
     def __init__(self, excepted, got):
-        super().__init__(f"InvalidStatusType. Expected: {excepted} type got: {got} type.")
+        super().__init__(
+            f"InvalidStatusType. Expected: {excepted} type got: {got} type."
+        )
 
 
 class MessagesLimitException(SelfBotClientException):
-
     def __init__(self, message: str):
         super().__init__(message)
```

### Comparing `asynccore-1.2.0/asynccore/gateway/enums.py` & `asynccore-1.2.1/asynccore/gateway/enums.py`

 * *Files identical despite different names*

### Comparing `asynccore-1.2.0/asynccore/gateway/errors.py` & `asynccore-1.2.1/asynccore/gateway/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from ..errors import SelfBotClientException
 
 if TYPE_CHECKING:
-    from ..user import UserClient
+    pass
 
 
 class MissingEventName(SelfBotClientException):
-
     def __init__(self, func: callable):  # pyright: ignore
         super().__init__(f"Missing event_name value in {func}")
 
 
 class InvalidEventName(SelfBotClientException):
-
     def __init__(self, name: str):  # pyright: ignore
         super().__init__(f"Event name: {name} is not available.")
 
 
 class FunctionIsNotCoroutine(SelfBotClientException):
-
     def __init__(self, function: callable):  # pyright: ignore
         super().__init__(f"Function: {function} is not coroutine.")
 
 
 class GatewayNotConnected(SelfBotClientException):
-
     def __init__(self, text: str = None):  # pyright: ignore
         super().__init__(text)
```

### Comparing `asynccore-1.2.0/asynccore/gateway/event.py` & `asynccore-1.2.1/asynccore/gateway/event.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,29 +17,30 @@
 class EventHandler:
     """
     EventHanlder is responsible for handling all evnets with :class:`Events`
 
     :param response: Get the event name and data
     :param kwargs: Pass in the user, client and gateway objects
     """
-    def __init__(self, response: GatewayResponse, **kwargs):
 
+    def __init__(self, response: GatewayResponse, **kwargs):
         self.response: GatewayResponse = response
 
         self.user: UserClient = kwargs["user"]
         self.client: Client = kwargs["client"]
         self.gateway: Gateway = kwargs["gateway"]
         self.connection: GatewayConnection = kwargs["connection"]
 
         self.event_name: str = self.reformat_event_name(
             event_name=response.event_name
         )  # pyright: ignore
 
-        self.available_events: dict[str, tuple] = {
-        }  # Format: "Event name": (default_callback, *args)
+        self.available_events: dict[
+            str, tuple
+        ] = {}  # Format: "Event name": (default_callback, *args)
 
         for event in Events:
             func = getattr(self.client, event.value)
 
             if event.name == "READY":
                 args: tuple = (func, self.user)
             else:
@@ -51,18 +52,19 @@
         if self.response.op == 10:
             latency: int = self.response.data["heartbeat_interval"] / 1000
             self.connection._pulse = latency
             await self.connection.login()
             await self.connection.begin_presence()
 
         elif self.response.event_name == "GUILD_MEMBER_LIST_UPDATE":
-
             if self.response.data["ops"][0]["op"] == "SYNC" and self.connection.func:
                 self.connection._times = 0
-                await self.connection.func(self.response.data, self.connection._func_limit)
+                await self.connection.func(
+                    self.response.data, self.connection._func_limit
+                )
 
             elif self.response.data["ops"][0]["op"] == "INVALIDATE":
                 self.connection._times += 1
                 if self.connection._times >= 5:
                     self.connection._times = 0
                     self.connection.func = None
                     self.user._members_end = False
@@ -90,28 +92,38 @@
 
             if not event_args:
                 return False
 
         if not self.available_events.get(self.event_name):
             return False
 
-        event_callback: Optional[Callable] = self.gateway.events.get(self.event_name)  # pyright: ignore
+        event_callback: Optional[Callable] = self.gateway.events.get(
+            self.event_name
+        )  # pyright: ignore
 
-        default_event_callback: Optional[Callable] = self.available_events[self.event_name][0]  # pyright: ignore
+        default_event_callback: Optional[Callable] = self.available_events[
+            self.event_name
+        ][
+            0
+        ]  # pyright: ignore
         if not event_args:
-            event_args: Optional[tuple] = self.available_events[self.event_name][1::]  # pyright: ignore
+            event_args: Optional[tuple] = self.available_events[self.event_name][
+                1::
+            ]  # pyright: ignore
 
         if event_callback:
             self.client.loop.create_task(
                 event_callback(*event_args) if event_args else event_callback()
             )
         else:
             if iscoroutinefunction(default_event_callback):
                 self.client.loop.create_task(
-                    default_event_callback(*event_args) if event_args else default_event_callback()
+                    default_event_callback(*event_args)
+                    if event_args
+                    else default_event_callback()
                 )
             else:
                 raise FunctionIsNotCoroutine(default_event_callback)
 
         return True
 
     @staticmethod
```

### Comparing `asynccore-1.2.0/asynccore/gateway/gateway.py` & `asynccore-1.2.1/asynccore/gateway/gateway.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional, Callable
 from time import time
-
+from socket import gaierror
 from json import dumps
-from asyncio import AbstractEventLoop, sleep, Queue, create_task, gather, Task, iscoroutinefunction
-import socket
-from websockets import connect, WebSocketClientProtocol, ConnectionClosed  # pyright: ignore
+
+from asyncio import (
+    AbstractEventLoop,
+    sleep,
+    Queue,
+    create_task,
+    gather,
+    Task,
+    iscoroutinefunction,
+)
+
+from websockets import (
+    connect,  # pyright: ignore
+    WebSocketClientProtocol,  # pyright: ignore
+    ConnectionClosed,  # pyright: ignore
+)
 
 from .response import GatewayResponse
 from .errors import MissingEventName, InvalidEventName, FunctionIsNotCoroutine
 from .event import EventHandler
 from .enums import Events
 
 if TYPE_CHECKING:
@@ -35,16 +48,17 @@
     The gateway class is responsible for connecting all users to the discord's gateway.
 
     :param client: Library main client
     :param gateway_url: gateway_url to connect to the discord gateway
     :param activity: Set the activity of the user
     """
 
-    def __init__(self, client: Client, gateway_url: str, activity: Optional[ActivityBuilder]):
-
+    def __init__(
+        self, client: Client, gateway_url: str, activity: Optional[ActivityBuilder]
+    ):
         self.client: Client = client
         self.gateway_url: str = gateway_url
         self.activity = activity
 
         self.events: dict[str, Callable] = {}
 
         self.supportted_events: list[str] = [event.value for event in Events]
@@ -65,17 +79,21 @@
 
         :param reconnect: Determine whether or not the connection is a reconnection
         """
 
         tasks: list[Task] = []
 
         for user in self.client.users:
-            connection = GatewayConnection(client=self.client, user=user,
-                                           gateway=self, activity=self.activity,
-                                           reconnect=reconnect)
+            connection = GatewayConnection(
+                client=self.client,
+                user=user,
+                gateway=self,
+                activity=self.activity,
+                reconnect=reconnect,
+            )
 
             task: Task = self.client.loop.create_task(connection.run(self.gateway_url))
             tasks.append(task)
 
         async def run():
             await gather(*tasks)
 
@@ -112,17 +130,22 @@
     :param client: Store the client object in the gateway connection
     :param user: Store the user object in the gateway connection,
     :param gateway: Create a new gateway connection
     :param activity: Set the activity of the user
     :param reconnect: Determine whether the userx should reconnect or not
     """
 
-    def __init__(self, client: Client, user: UserClient, gateway: Gateway,
-                 activity: Optional[ActivityBuilder], reconnect: bool):
-
+    def __init__(
+        self,
+        client: Client,
+        user: UserClient,
+        gateway: Gateway,
+        activity: Optional[ActivityBuilder],
+        reconnect: bool,
+    ):
         self.client: Client = client
         self.user: UserClient = user
         self.activity: Optional[ActivityBuilder] = activity
         self.reconnect: bool = reconnect
 
         self._gateway: Gateway = gateway
         self._loop: AbstractEventLoop = client.loop
@@ -148,31 +171,36 @@
             2) Sending requests to Discord (self._send_request())
             3) Pinging Discord every x seconds (self._ping_loop())
 
         :param gateway_url: url to connect
         """
 
         try:
-            async with connect(gateway_url, extra_headers=self.get_headers) as websocket:
+            async with connect(
+                gateway_url, extra_headers=self.get_headers
+            ) as websocket:
                 self.websocket: WebSocketClientProtocol = websocket
 
                 if self.client.logger._status:
                     self.client.logger.info(f"Successfully connected to {gateway_url}")
 
                 tasks: list[Task] = [
                     create_task(self._receive_response()),
                     create_task(self._send_request()),
-                    create_task(self._ping_loop())]
+                    create_task(self._ping_loop()),
+                ]
 
                 for task in tasks:
                     await task
 
         except ConnectionClosed:
             if self.client.logger._status:
-                self.client.logger.error(f"Connection: {self._gateway.gateway_url} Closed. Trying to resume.")
+                self.client.logger.error(
+                    f"Connection: {self._gateway.gateway_url} Closed. Trying to resume."
+                )
 
             if not self._resume_gateway or not self._session_id or not self.reconnect:
                 return
 
             await self.resume()
 
     async def resume(self):
@@ -188,37 +216,44 @@
     async def resume_connection(self):
         """
         The resume_connection function is used to resume a connection with the Discord Gateway.
         It does this by sending a RESUME payload to the gateway.
         """
 
         try:
-            async with connect(self._resume_gateway, extra_headers=self.get_headers) as websocket:
+            async with connect(
+                self._resume_gateway, extra_headers=self.get_headers
+            ) as websocket:
                 self.websocket: WebSocketClientProtocol = websocket
 
                 if self.client.logger._status:
-                    self.client.logger.info(f"Successfully connected to: {self._resume_gateway}")
+                    self.client.logger.info(
+                        f"Successfully connected to: {self._resume_gateway}"
+                    )
 
                 tasks: list[Task] = [
                     create_task(self._send_resume()),
                     create_task(self._receive_response()),
                     create_task(self._send_request()),
-                    create_task(self._ping_loop())]
+                    create_task(self._ping_loop()),
+                ]
 
                 for task in tasks:
                     await task
-        except socket.gaierror:
+        except gaierror:
             pass
 
         except ConnectionClosed:
             if not self._resume_gateway or not self._session_id:
                 return
 
             if self.client.logger._status:
-                self.client.logger.error(f"Connection: {self._gateway.gateway_url} Closed. Trying to resume.")
+                self.client.logger.error(
+                    f"Connection: {self._gateway.gateway_url} Closed. Trying to resume."
+                )
 
             await self.resume()
 
     @property
     def get_headers(self) -> dict:
         """
         The get_headers function returns a dictionary of headers that are used to make the request.
@@ -226,15 +261,15 @@
 
         headers = {
             "Accept-Encoding": "gzip, deflate, br",
             "Accept-Language": "en-US,en;q=0.9",
             "Cache-Control": "no-cache",
             "Pragma": "no-cache",
             "Sec-WebSocket-Extensions": "permessage-deflate; client_max_window_bits",
-            "User-Agent": "Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:47.0) Gecko/20100101 Firefox/47.0"
+            "User-Agent": "Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:47.0) Gecko/20100101 Firefox/47.0",
         }
         return headers
 
     async def begin_presence(self):
         """
         The begin_presence function is used to send the initial presence payload to Discord.
         This function is called when the client connects and has received a READY payload from Discord.
@@ -242,24 +277,26 @@
         """
 
         if self.activity:
             payload = {
                 "op": 3,
                 "d": {
                     "since": time(),
-                    "activities": [{
-                        "name": self.activity.activity_name,
-                        "type": self.activity.activity_type,
-                        "created_at": time(),
-                        "since": 0,
-                        "details": self.activity.activity_details
-                    }],
+                    "activities": [
+                        {
+                            "name": self.activity.activity_name,
+                            "type": self.activity.activity_type,
+                            "created_at": time(),
+                            "since": 0,
+                            "details": self.activity.activity_details,
+                        }
+                    ],
                     "status": self.activity.user_status,
                     "afk": False,
-                }
+                },
             }
             await self.send(payload)
 
     async def login(self) -> None:
         """
         The login function is used to send the login request to Discord.
         It takes no arguments, and returns nothing.
@@ -276,22 +313,18 @@
                 device: str = f"Discord {os}"
 
         request = {
             "op": 2,
             "d": {
                 "token": self.user.token,
                 "capabilities": 4093,
-                "properties": {
-                    "os": os,
-                    "browser": browser,
-                    "device": device
-                },
-                "compress": False
+                "properties": {"os": os, "browser": browser, "device": device},
+                "compress": False,
             },
-            "intents": 98047
+            "intents": 98047,
         }
         await self.send(request)
 
     async def _receive_response(self):
         """
         The _receive_response function is a coroutine that receives responses from the gateway.
         It handles all events and dispatches them to their respective handlers. It also handles
@@ -309,29 +342,34 @@
                 self._last_sequence = gateway_response.sequence
 
             if gateway_response.event:
                 if gateway_response.event_name == "READY":
                     if self.func:
                         continue
 
-                    self._resume_gateway = gateway_response.data.get("resume_gateway_url")
+                    self._resume_gateway = gateway_response.data.get(
+                        "resume_gateway_url"
+                    )
 
             handler = EventHandler(
                 response=gateway_response,
                 client=self.client,
                 user=self.user,
                 gateway=self._gateway,
-                connection=self
+                connection=self,
             )
 
-            def check_event_type():
-                return gateway_response.event_name in ("GUILD_APPLICATION_COMMANDS_UPDATE",
-                                                       "GUILD_MEMBER_LIST_UPDATE") or gateway_response.op == 10
+            def check_event_type(resp: GatewayResponse):
+                return (
+                    resp.event_name
+                    in ("GUILD_APPLICATION_COMMANDS_UPDATE", "GUILD_MEMBER_LIST_UPDATE")
+                    or resp.op == 10
+                )
 
-            if check_event_type():
+            if check_event_type(gateway_response):
                 await handler.handle_abstract_events()
             else:
                 await handler.handle_event()
 
     async def _send_request(self):
         """
         The _send_request function is a coroutine that sends requests to the server.
@@ -351,18 +389,15 @@
         It sends a ping request to Discord every self._pulse seconds, which is set to 5 by default.
         The purpose of this function is to keep the connection alive and prevent it from timing out.
         """
 
         while True:
             await sleep(self._pulse)
 
-            ping_request: dict = {
-                "op": 1,
-                "d": time()
-            }
+            ping_request: dict = {"op": 1, "d": time()}
 
             await self.send(ping_request)
 
     async def _send_resume(self):
         """
         The _send_resume function is used to send a resume payload to the Discord gateway.
         This function is called when the websocket connection has been lost and needs to be re-established.
@@ -370,26 +405,28 @@
         """
 
         payload: dict = {
             "op": 6,
             "d": {
                 "token": self.user.token,
                 "session_id": self._session_id,
-                "seq": self._last_sequence
-            }
+                "seq": self._last_sequence,
+            },
         }
         await self.send(payload)
 
     async def send(self, request):
         """
         The send function is a coroutine that takes in a request and puts it into the queue.
         """
         await self._queue.put(request)
 
-    async def application_update_request(self, request: dict, func: Callable, limit: Optional[int] = None):
+    async def application_update_request(
+        self, request: dict, func: Callable, limit: Optional[int] = None
+    ):
         """
         The application_update_request function is a coroutine that takes in a request and function.
         The request is put into the queue, and the function is set to be called when it's time to process
         the request.
 
         :param request: Pass the request to the application_update_request function
         :param func: Store the function that will be called when a response is received
```

### Comparing `asynccore-1.2.0/asynccore/gateway/response.py` & `asynccore-1.2.1/asynccore/gateway/response.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,30 +12,29 @@
     The class that formats the raw discord response.
 
     :param data: Store the raw data from discord
     :param user: Pass the user object to the response
 
     :ivar user: The object of the user who received the response.
     :vartype user: :class:`asynccore.user.UserClient`
-    
+
     :ivar event: Is the response an event
     :vartype event: :class:`bool`
 
     :ivar op: Op of discord response
     :vartype op: :class:`int`
 
     :ivar data: Response data
     :vartype data: :class:`dict`
 
     :ivar sequence: Discord sequence
     :vartype sequence: :class:`int`
     """
 
     def __init__(self, data: str, user: UserClient):
-
         self.user: UserClient = user
         self.data: dict = self.format_data(data)
         self.event: bool = False
 
         self.op: int = self.data["op"]  # pylint: disable=invalid-name
 
         if self.op == 0:
@@ -57,12 +56,17 @@
 
         :param data: Pass in the data that is being formatted
         """
         return loads(data)
 
     def __repr__(self):
         if self.event:
-            return f"<GatewayResponse(user={self.user},event_type={self.event_name}, " \
-                 f"op={self.op}, " f"sequence={self.sequence}, data={self.data})>"
-
-        return f"<GatewayResponse(user={self.user}, op={self.op}, " \
-               f"sequence={self.sequence}, data={self.data})>"
+            return (
+                f"<GatewayResponse(user={self.user},event_type={self.event_name}, "
+                f"op={self.op}, "
+                f"sequence={self.sequence}, data={self.data})>"
+            )
+
+        return (
+            f"<GatewayResponse(user={self.user}, op={self.op}, "
+            f"sequence={self.sequence}, data={self.data})>"
+        )
```

### Comparing `asynccore-1.2.0/asynccore/http.py` & `asynccore-1.2.1/asynccore/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 if TYPE_CHECKING:
     from .client import Client
 
 __all__: tuple[str, ...] = ("HTTPClient", "ClientResponse", "CustomSession")
 
 
 class CustomSession(ClientSession):
-
     def __init__(self, logger: Logger, *args: Any, **kwargs: Any):
         """
         The __init__ function sets up all of the variables that are needed for other functions to work properly.
         The super() function calls __init__ from the parent class, which in this case is ClientSession.
 
         :param logger: Pass the logger object to the class
         :param *args: Pass any additional arguments to the superclass
@@ -71,22 +70,28 @@
                 _json: dict = {}
 
             if isinstance(_json, dict):
                 message: Optional[str] = _json.get("message")
                 if message and "You need to verify" in message and self.users:
                     for user in self.users:
                         if user.token == token:
-                            self.logger.error(f"It seems that your account has been blocked.\n-> Account: {user}")
+                            self.logger.error(
+                                f"It seems that your account has been blocked.\n-> Account: {user}"
+                            )
                     response.status = 901
 
         if response.headers.get("Retry-After"):
-
-            seconds = int(response.headers.get("Retry-After")) + self.ratelimit_additional_cooldown  # pyright: ignore
+            seconds = (
+                int(response.headers["Retry-After"])
+                + self.ratelimit_additional_cooldown
+            )
             if self.logger_status:
-                self.logger.warning(f"Ratelimit has been reached. Awaiting {seconds} seconds before next request.")
+                self.logger.warning(
+                    f"Ratelimit has been reached. Awaiting {seconds} seconds before next request."
+                )
 
             await sleep(seconds)
         else:
             await sleep(self.request_latency)
 
         return response
 
@@ -103,61 +108,66 @@
     :param ratelimit_additional_cooldown: Add a cooldown to the ratelimit
     :param client: Client object needed to connect to gateway
     :param activity: The argument with type :class:`AcivityBuilder` is responsible for account activity.
     :param startup_cache: Enable or disable cache fetching at program startup
     """
 
     def __init__(
-            self,
-            api_version: API_VERSION,
-            loop: Union[AbstractEventLoop, None],
-            logger: bool,
-            request_latency: float,
-            ratelimit_additional_cooldown: float,
-            client: Client,
-            activity: Optional[ActivityBuilder],
-            startup_cache: bool
+        self,
+        api_version: API_VERSION,
+        loop: Union[AbstractEventLoop, None],
+        logger: bool,
+        request_latency: float,
+        ratelimit_additional_cooldown: float,
+        client: Client,
+        activity: Optional[ActivityBuilder],
+        startup_cache: bool,
     ):
-
         if api_version not in (9, 10):
             raise UnSupportedApiVersion
 
         self.request_latency: float = request_latency
         self.ratelimit_additional_cooldown: float = ratelimit_additional_cooldown
         self.start = time()
 
         self.api_version: int = api_version
         self.endpoint: str = Discord.ENDPOINT.value.format(self.api_version)
-        self.endpoint_gateway: str = Discord.ENDPONT_GATEWAY.value.format(self.api_version)
+        self.endpoint_gateway: str = Discord.ENDPONT_GATEWAY.value.format(
+            self.api_version
+        )
 
         self.loop: AbstractEventLoop = loop if loop else get_event_loop()
 
         self._tokens: Union[str, list, None] = None
         self._logger_status: bool = logger
 
         self.logger: Logger.logger = Logger().logger  # pyright: ignore
         self.logger._status = self._logger_status
         self.session: Union[CustomSession, None] = None  # pyright: ignore
 
         self.users: list[UserClient] = []
         self.loop.run_until_complete(self.create_session())
 
         self.use_cache: bool = startup_cache
-        self.gateway: Gateway = Gateway(client=client, gateway_url=self.endpoint_gateway, activity=activity)
+        self.gateway: Gateway = Gateway(
+            client=client, gateway_url=self.endpoint_gateway, activity=activity
+        )
 
     async def create_session(self) -> None:
         """
         The create_session function is used to create a new session for the Client.
         The session object contains all of the information that we need in order to connect with Discord's API.
         """
 
-        self.session: CustomSession = CustomSession(self.logger,
-                                                    latency=self.request_latency,
-                                                    additional_cooldown=self.ratelimit_additional_cooldown,
-                                                    users=self.users)
+        self.session: CustomSession = CustomSession(
+            self.logger,
+            latency=self.request_latency,
+            additional_cooldown=self.ratelimit_additional_cooldown,
+            users=self.users,
+        )
 
     def _check_tokens(self, tokens: Union[list[str], str]) -> None:  # pyright: ignore
         """
         The _check_tokens function is used to check if the tokens provided are valid.
         If they are, then it will add them to the users list. If not, then it will delete them from the list.
 
         :param tokens: Tokens to check
@@ -167,31 +177,36 @@
             _url: str = self.endpoint + "users/@me"
             for token in tokens:
                 header: AUTH_HEADER = AUTH_HEADER(authorization=token)
                 response: ClientResponse = await self.session.get(_url, headers=header)
                 if response.status != 200:
                     if self._logger_status:
                         self.logger.warning(
-                            f"An invalid token has been provided: {token} | The token will be automatically deleted")
+                            f"An invalid token has been provided: {token} | The token will be automatically deleted"
+                        )
 
                 else:
                     data: dict = await response.json()
                     data["token"] = token
                     data["loop"] = self.loop
                     data["endpoint"] = self.endpoint
                     data["endpoint_gateway"] = self.endpoint_gateway
 
                     self.users.append(UserClient(data, self.session))
 
             if self._logger_status:
-                self.logger.info(f"Checking of tokens successfully completed | Loaded ({len(self.users)}) tokens\n")
+                self.logger.info(
+                    f"Checking of tokens successfully completed | Loaded ({len(self.users)}) tokens\n"
+                )
 
             if self.use_cache:
                 if self._logger_status:
-                    self.logger.debug(f"Fetching cache for {len(self.users)} selfbots...")
+                    self.logger.debug(
+                        f"Fetching cache for {len(self.users)} selfbots..."
+                    )
 
                 for user in self.users:
                     await user.cache.startup_cache()
                     await sleep(0.5)
 
                 if self._logger_status:
                     seconds: str = str(time() - self.start)[0:3]
@@ -218,16 +233,21 @@
         the awaitable completes. This is useful for running tasks in parallel with other code.
 
         :param function: Specify the coroutine
         """
 
         self.loop.run_until_complete(function)
 
-    async def request(self, url: str, method: METHOD, headers: Optional[dict] = None,
-                      data: Optional[dict] = None) -> ClientResponse:
+    async def request(
+        self,
+        url: str,
+        method: METHOD,
+        headers: Optional[dict] = None,
+        data: Optional[dict] = None,
+    ) -> ClientResponse:
         """
         The request function is used to send a request to the API.
 
         :param url: Specify the url of the request
         :param method: Specify the type of request being sent
         :param headers: Pass in a dictionary of headers to be sent with the request
         :param data: Send data to the api
@@ -237,11 +257,13 @@
             raise InvalidMethodType(method)
 
         _url: str = self.endpoint + url
 
         if self._logger_status:
             self.logger.debug(f"Sending request: {method} -> {_url}")
 
-        response: ClientResponse = await self.session.request(method=method, url=_url, headers=headers, json=data)
+        response: ClientResponse = await self.session.request(
+            method=method, url=_url, headers=headers, json=data
+        )
         response.raise_for_status()
 
         return response
```

### Comparing `asynccore-1.2.0/asynccore/logger.py` & `asynccore-1.2.1/asynccore/logger.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 
     __slots__ = ("logger", "_status", "debug", "error", "warning")
 
     log_level: int = DEBUG
     log_format: str = "%(log_color)s%(levelname)s | %(asctime)s > %(message)s"
 
     def __init__(self):
-
-        formatter = ColoredFormatter(self.log_format, datefmt='%H:%M:%S')
+        formatter = ColoredFormatter(self.log_format, datefmt="%H:%M:%S")
         stream = StreamHandler()
         stream.setLevel(self.log_level)
         stream.setFormatter(formatter)
 
-        self.logger = getLogger('Logger')
+        self.logger = getLogger("Logger")
         self.logger.setLevel(self.log_level)
         self.logger.addHandler(stream)
         self.logger._status = True  # pyright: ignore
```

### Comparing `asynccore-1.2.0/asynccore/permissionbuilder.py` & `asynccore-1.2.1/asynccore/permissionbuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
     :param args: PermissionType values
     """
 
     __slots__ = ("value",)
 
     def __init__(self, *args: Permissions) -> None:
-
         self.value: int = 0
 
         for permission in args:
             if isinstance(permission, Permissions):
                 self.value += permission.value
 
     def __repr__(self):
```

### Comparing `asynccore-1.2.0/asynccore/tasks.py` & `asynccore-1.2.1/asynccore/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,17 @@
         """
         The run_until_complete function is used to run a task until it's complete.
         This function will also wait for the main loop to finish before executing any of its tasks.
         """
 
         if self._loop.is_running():
             if self._client.logger._status:
-                self._client.logger.debug("The main loop is already up and running. I'm waiting for it to finish.")
+                self._client.logger.debug(
+                    "The main loop is already up and running. I'm waiting for it to finish."
+                )
 
         while self._loop.is_running():
             sleep(1)
 
         for _ in self._tasks:
             self._loop.run_until_complete(_)
```

### Comparing `asynccore-1.2.0/asynccore/user.py` & `asynccore-1.2.1/asynccore/user.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from aiohttp import ClientResponse
 
 from .typings import AUTH_HEADER, RGB_COLOR, MESSAGE_REFERENCE
 from .logger import Logger
 from .enums import ChannelType
 
 from .permissionbuilder import PermissionBuilder
+from .gateway.errors import GatewayNotConnected
 from .errors import MessagesLimitException
 from .cache import Cache
 
 if TYPE_CHECKING:
     from .gateway.gateway import GatewayConnection
     from .http import CustomSession
 
@@ -40,28 +41,30 @@
         self._members_end: bool = True
 
         self.token: str = self.data["token"]
         self.name: str = self.data["username"]
         self.discriminator: str = f"#{self.data['discriminator']}"
         self.id: int = self.data["id"]
 
-        self._auth_header: AUTH_HEADER = AUTH_HEADER(
-            authorization=self.token
-        )
+        self._auth_header: AUTH_HEADER = AUTH_HEADER(authorization=self.token)
 
         self.loop: AbstractEventLoop = data["loop"]
         self.cache: Cache = Cache(user=self, session=session, endpoint=self._endpoint)
         self.gateway_connection: Optional[GatewayConnection] = None
 
     def __repr__(self):
         return f"<UserClient(name={self.name}, discriminator={self.discriminator}, id={self.id})>"
 
-    async def reply_message(self, channel_id: int, message_id: int,
-                            message_content: str, mention_author: bool = True) -> ClientResponse:
-
+    async def reply_message(
+        self,
+        channel_id: int,
+        message_id: int,
+        message_content: str,
+        mention_author: bool = True,
+    ) -> ClientResponse:
         """
         The reply_message function is used to reply to a message in a channel.
 
         :param channel_id: Specify the channel to send the message in
         :param message_id: message id of the message that you want to reply to
         :param message_content: A message content
         :param mention_author: Determine whether or not to mention the author of the message
@@ -69,155 +72,167 @@
 
         _url = self._endpoint + f"channels/{channel_id}/messages"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: POST -> {_url}")
 
         message_reference = MESSAGE_REFERENCE(
-            message_id=message_id,
-            channel_id=channel_id
+            message_id=message_id, channel_id=channel_id
         )
 
         payload: dict = {
             "content": message_content,
-            "message_reference": message_reference
+            "message_reference": message_reference,
         }
 
         if not mention_author:
-            _message_response: ClientResponse = await self.get_message(channel_id, message_id)
+            _message_response: ClientResponse = await self.get_message(
+                channel_id, message_id
+            )
             if _message_response.status == 200:
-                _message_data: list[dict] = await _message_response.json()  # pyright: ignore
-                _message_data: dict = _message_data[0]
-                _message_author_id: int = _message_data["author"]["id"]
-
-                payload["allowed_mentions"] = {
-                    "users": [f"{_message_author_id}"]
-                }
+                _message_data: list[
+                    dict
+                ] = await _message_response.json()  # pyright: ignore
+                message_data: dict = _message_data[0]
+                _message_author_id: int = message_data["author"]["id"]
+
+                payload["allowed_mentions"] = {"users": [f"{_message_author_id}"]}
 
             else:
-                payload["allowed_mentions"] = {
-                    "parse": ["users"]
-                }
+                payload["allowed_mentions"] = {"parse": ["users"]}
 
         response: ClientResponse = await self._session.request(
-            method="POST", url=_url, headers=self._auth_header, json=payload)
+            method="POST", url=_url, headers=self._auth_header, json=payload
+        )
 
         if response.status not in (200, 429) and self._logger._status:
             self._logger.warning(
-                f"Request POST channels/{channel_id}/messages failed.\n -> {self} {await response.json()}")
+                f"Request POST channels/{channel_id}/messages failed.\n -> {self} {await response.json()}"
+            )
 
         return response
 
-    async def send_message(self, channel_id: int, message_content: str) -> ClientResponse:
-
+    async def send_message(
+        self, channel_id: int, message_content: str
+    ) -> ClientResponse:
         """
         The send_message function sends a message to the specified channel.
 
         :param channel_id: Specify the channel to send the message to
         :param message_content: content of the message
         """
 
         _url = self._endpoint + f"channels/{channel_id}/messages"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: POST -> {_url}")
 
-        payload: dict = {
-            "content": message_content
-        }
+        payload: dict = {"content": message_content}
 
         response: ClientResponse = await self._session.request(
-            method="POST", url=_url, headers=self._auth_header, json=payload)
+            method="POST", url=_url, headers=self._auth_header, json=payload
+        )
 
         if response.status not in (200, 429) and self._logger._status:
             self._logger.warning(
-                f"Request POST channels/{channel_id}/messages failed.\n -> {self} {await response.json()}")
+                f"Request POST channels/{channel_id}/messages failed.\n -> {self} {await response.json()}"
+            )
 
         return response
 
-    async def edit_message(self, channel_id: int, message_id: int, message_content: str) -> ClientResponse:
+    async def edit_message(
+        self, channel_id: int, message_id: int, message_content: str
+    ) -> ClientResponse:
         """
         The edit_message function allows you to edit a message.
 
         :param channel_id: Specify the channel id of the message you want to edit
         :param message_id: id the message to edit
         :param message_content: Edit the message content
         """
 
         _url = self._endpoint + f"/channels/{channel_id}/messages/{message_id}"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: PATCH -> {_url}")
 
-        payload: dict = {
-            "content": message_content
-        }
+        payload: dict = {"content": message_content}
 
         response: ClientResponse = await self._session.request(
-            method="PATCH", url=_url, headers=self._auth_header, json=payload)
+            method="PATCH", url=_url, headers=self._auth_header, json=payload
+        )
 
         if response.status not in (200, 429) and self._logger._status:
             self._logger.error(
                 f"Request PATCH /channels/{channel_id}/messages/{message_id} failed."
-                f"\n -> {self} {await response.json()}")
+                f"\n -> {self} {await response.json()}"
+            )
 
         return response
 
     async def get_message(self, channel_id: int, message_id: int) -> ClientResponse:
         """
         The get_message function is used to get a message from a channel.
 
         :param channel_id: Specify the channel id of the message you want to get
         :param message_id: Get the message around that id
         """
 
         # Since the normal get_message endpoint returns the message
         # "Only bots can use this endpoint" we get the message in a different way
 
-        _url = self._endpoint + f"channels/{channel_id}/messages?limit=1&around={message_id}"
+        _url = (
+            self._endpoint
+            + f"channels/{channel_id}/messages?limit=1&around={message_id}"
+        )
 
         if self._logger._status:
             self._logger.debug(f"Sending request: GET -> {_url}")
 
         response: ClientResponse = await self._session.request(
-            method="GET", url=_url, headers=self._auth_header)
+            method="GET", url=_url, headers=self._auth_header
+        )
 
         if response.status not in (200, 429) and self._logger._status:
             self._logger.error(
                 f"Request GET channels/{channel_id}/messages?limit=1&around={message_id} failed."
-                f"\n -> {self} {await response.json()}")
+                f"\n -> {self} {await response.json()}"
+            )
 
         return response
 
     async def get_messages(self, channel_id: int, limit: int = 100) -> ClientResponse:
         """
         The get_messages function is used to retrieve a list of message objects from the channel.
 
         :param channel_id: Specify which channel to get the messages from
         :param limit: Limit the number of messages returned
         """
         if limit > 100:
             raise MessagesLimitException(
                 "Unfortunately, but discord only allows a maximum of 100 recent messages to be returned. "
-                f"You specified limit={limit}")
+                f"You specified limit={limit}"
+            )
 
         if limit < 2:
             raise MessagesLimitException("Message limit must be greater than 1")
 
         _url = self._endpoint + f"channels/{channel_id}/messages?limit={limit}"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: GET -> {_url}")
 
         response: ClientResponse = await self._session.request(
-            method="GET", url=_url, headers=self._auth_header)
+            method="GET", url=_url, headers=self._auth_header
+        )
 
         if response.status not in (200, 429) and self._logger._status:
             self._logger.error(
-                f"Request GET channels/{channel_id}/messages failed.\n -> {self} {response.status}")
+                f"Request GET channels/{channel_id}/messages failed.\n -> {self} {response.status}"
+            )
 
         return response
 
     async def delete_message(self, channel_id: int, message_id: int) -> ClientResponse:
         """
         The delete_message function deletes a message from the specified channel.
 
@@ -227,20 +242,22 @@
 
         _url = self._endpoint + f"channels/{channel_id}/messages/{message_id}"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: DELETE -> {_url}")
 
         response: ClientResponse = await self._session.request(
-            method="DELETE", url=_url, headers=self._auth_header)
+            method="DELETE", url=_url, headers=self._auth_header
+        )
 
         if response.status not in (204, 429) and self._logger._status:
             self._logger.error(
                 f"Request DELETE channels/{channel_id}/messages/{message_id} failed."
-                f"\n -> {self} {await response.json()}")
+                f"\n -> {self} {await response.json()}"
+            )
 
         return response
 
     async def delete_channel(self, channel_id: int) -> ClientResponse:
         """
         The delete_channel function deletes a channel from the server.
 
@@ -249,25 +266,34 @@
 
         _url = self._endpoint + f"channels/{channel_id}"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: DELETE -> {_url}")
 
         response: ClientResponse = await self._session.request(
-            method="DELETE", url=_url, headers=self._auth_header)
+            method="DELETE", url=_url, headers=self._auth_header
+        )
 
         if response.status not in (200, 429) and self._logger._status:
             self._logger.error(
-                f"Request DELETE channels/{channel_id} failed.\n -> {self} {await response.json()}")
+                f"Request DELETE channels/{channel_id} failed.\n -> {self} {await response.json()}"
+            )
 
         return response
 
-    async def create_channel(self, guild_id: int, name: str, channel_type: ChannelType,
-                             topic: Optional[str] = None, user_limit: Optional[int] = None,
-                             position: Optional[int] = None, nsfw: Optional[bool] = False) -> ClientResponse:
+    async def create_channel(
+        self,
+        guild_id: int,
+        name: str,
+        channel_type: ChannelType,
+        topic: Optional[str] = None,
+        user_limit: Optional[int] = None,
+        position: Optional[int] = None,
+        nsfw: Optional[bool] = False,
+    ) -> ClientResponse:
         """
         The create_channel function creates a channel in the specified guild.
 
         :param guild_id: Specify the guild id of the server you want to create a channel in
         :param name: Specify the name of the channel
         :param channel_type: Specify what type of channel you want to create
         :param topic: Set the topic of the channel
@@ -283,23 +309,25 @@
 
         payload: dict = {
             "name": name,
             "type": channel_type.value,
             "topic": topic,
             "user_limit": user_limit,
             "position": position,
-            "nsfw": nsfw
+            "nsfw": nsfw,
         }
 
         response: ClientResponse = await self._session.request(
-            method="POST", url=_url, headers=self._auth_header, json=payload)
+            method="POST", url=_url, headers=self._auth_header, json=payload
+        )
 
         if response.status not in (201, 429) and self._logger._status:
             self._logger.error(
-                f"Request POST /guilds/{guild_id}/channels failed.\n -> {self} {await response.json()}")
+                f"Request POST /guilds/{guild_id}/channels failed.\n -> {self} {await response.json()}"
+            )
 
         return response
 
     async def get_channels(self, guild_id: int) -> ClientResponse:
         """
         The get_channels function is a coroutine that takes in a guild_id and returns an ClientResponse object.
         The function can return the data of all channels on the server
@@ -309,19 +337,21 @@
 
         _url = self._endpoint + f"guilds/{guild_id}/channels"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: GET -> {_url}")
 
         response: ClientResponse = await self._session.request(
-            method="GET", url=_url, headers=self._auth_header)
+            method="GET", url=_url, headers=self._auth_header
+        )
 
         if response.status not in (200, 429) and self._logger._status:
             self._logger.error(
-                f"Request GET guilds/{guild_id}/channels failed.\n -> {self} {await response.json()}.")
+                f"Request GET guilds/{guild_id}/channels failed.\n -> {self} {await response.json()}."
+            )
 
         return response
 
     async def get_channel(self, channel_id: int) -> ClientResponse:
         """
         The get_channel function returns a channel data for the given channel ID.
 
@@ -330,29 +360,32 @@
 
         _url = self._endpoint + f"/channels/{channel_id}"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: GET -> {_url}")
 
         response: ClientResponse = await self._session.request(
-            method="GET", url=_url, headers=self._auth_header)
+            method="GET", url=_url, headers=self._auth_header
+        )
 
         if response.status not in (200, 429) and self._logger._status:
             self._logger.error(
-                f"Request GET /channels/{channel_id} failed.\n -> {self} {await response.json()}.")
+                f"Request GET /channels/{channel_id} failed.\n -> {self} {await response.json()}."
+            )
 
         return response
 
-    async def create_role(self,
-                          guild_id: int,
-                          name: str,
-                          color: Optional[RGB_COLOR] = None,
-                          hoist: Optional[bool] = False,
-                          permissions: Union[PermissionBuilder, int, None] = None) -> ClientResponse:
-
+    async def create_role(
+        self,
+        guild_id: int,
+        name: str,
+        color: Optional[RGB_COLOR] = None,
+        hoist: Optional[bool] = False,
+        permissions: Union[PermissionBuilder, int, None] = None,
+    ) -> ClientResponse:
         """
         The create_role function creates a role in the specified guild.
 
         :param guild_id: Specify the guild in which you want to create a role
         :param name: Set the name of the role
         :param color: Set the color of the role
         :param hoist: Determine whether the role should be displayed separately in the user list
@@ -375,23 +408,25 @@
         else:
             _permissions: int = permissions.value  # pyright: ignore
 
         json: dict = {
             "name": name,
             "hoist": hoist,
             "color": _color,
-            "permissions": _permissions
+            "permissions": _permissions,
         }
 
         response: ClientResponse = await self._session.request(
-            method="POST", url=_url, headers=self._auth_header, json=json)
+            method="POST", url=_url, headers=self._auth_header, json=json
+        )
 
         if response.status not in (200, 429) and self._logger._status:
             self._logger.error(
-                f"Request POST guilds/{guild_id}/roles failed.\n -> {self} {await response.json()}")
+                f"Request POST guilds/{guild_id}/roles failed.\n -> {self} {await response.json()}"
+            )
 
         return response
 
     async def get_roles(self, guild_id: int) -> ClientResponse:
         """
         get_roles returns a list of data with all the roles on the server
 
@@ -400,19 +435,21 @@
 
         _url = self._endpoint + f"guilds/{guild_id}/roles"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: GET -> {_url}")
 
         response: ClientResponse = await self._session.request(
-            method="GET", url=_url, headers=self._auth_header)
+            method="GET", url=_url, headers=self._auth_header
+        )
 
         if response.status not in (200, 429) and self._logger._status:
             self._logger.error(
-                f"Request GET guilds/{guild_id}/roles failed.\n -> {self} {await response.json()}")
+                f"Request GET guilds/{guild_id}/roles failed.\n -> {self} {await response.json()}"
+            )
 
         return response
 
     async def delete_role(self, guild_id: int, role_id: int) -> ClientResponse:
         """
         The delete_role function deletes a role from the guild.
 
@@ -422,19 +459,21 @@
 
         _url = self._endpoint + f"guilds/{guild_id}/roles/{role_id}"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: DELETE -> {_url}")
 
         response: ClientResponse = await self._session.request(
-            method="DELETE", url=_url, headers=self._auth_header)
+            method="DELETE", url=_url, headers=self._auth_header
+        )
 
         if response.status not in (204, 429) and self._logger._status:
             self._logger.error(
-                f"Request DELETE guilds/{guild_id}/roles/{role_id} failed.\n -> {self} {await response.json()}")
+                f"Request DELETE guilds/{guild_id}/roles/{role_id} failed.\n -> {self} {await response.json()}"
+            )
 
         return response
 
     async def get_guild_bans(self, guild_id: int) -> ClientResponse:
         """
         The get_guild_bans function returns a list of banned users in the guild.
 
@@ -443,19 +482,21 @@
         """
         _url = self._endpoint + f"guilds/{guild_id}/bans"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: GET -> {_url}")
 
         response: ClientResponse = await self._session.request(
-            method="GET", url=_url, headers=self._auth_header)
+            method="GET", url=_url, headers=self._auth_header
+        )
 
         if response.status not in (200, 429) and self._logger._status:
             self._logger.error(
-                f"Request GET guilds/{guild_id}/bans failed.\n -> {self} {await response.json()}")
+                f"Request GET guilds/{guild_id}/bans failed.\n -> {self} {await response.json()}"
+            )
 
         return response
 
     async def unban_member(self, guild_id: int, user_id: int) -> ClientResponse:
         """
         The unban_member function unban a user from the guild.
 
@@ -465,19 +506,21 @@
 
         _url = self._endpoint + f"guilds/{guild_id}/bans/{user_id}"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: DELETE -> {_url}")
 
         response: ClientResponse = await self._session.request(
-            method="DELETE", url=_url, headers=self._auth_header)
+            method="DELETE", url=_url, headers=self._auth_header
+        )
 
         if response.status not in (204, 429) and self._logger._status:
             self._logger.error(
-                f"Request DELETE guilds/{guild_id}/bans/{user_id} failed.\n -> {self} {await response.json()}")
+                f"Request DELETE guilds/{guild_id}/bans/{user_id} failed.\n -> {self} {await response.json()}"
+            )
 
         return response
 
     async def ban_member(self, guild_id: int, user_id: int) -> ClientResponse:
         """
         The ban_member function is used to ban a member from the guild.
 
@@ -487,19 +530,21 @@
 
         _url = self._endpoint + f"guilds/{guild_id}/bans/{user_id}"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: PUT -> {_url}")
 
         response: ClientResponse = await self._session.request(
-            method="PUT", url=_url, headers=self._auth_header)
+            method="PUT", url=_url, headers=self._auth_header
+        )
 
         if response.status not in (204, 429) and self._logger._status:
             self._logger.error(
-                f"Request PUT guilds/{guild_id}/bans/{user_id} failed.\n -> {self} {await response.json()}")
+                f"Request PUT guilds/{guild_id}/bans/{user_id} failed.\n -> {self} {await response.json()}"
+            )
 
         return response
 
     async def kick_member(self, guild_id: int, user_id: int) -> ClientResponse:
         """
         The kick_member function kicks a member from the guild.
 
@@ -509,19 +554,21 @@
 
         _url = self._endpoint + f"guilds/{guild_id}/members/{user_id}"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: DELETE -> {_url}")
 
         response: ClientResponse = await self._session.request(
-            method="DELETE", url=_url, headers=self._auth_header)
+            method="DELETE", url=_url, headers=self._auth_header
+        )
 
         if response.status not in (204, 429) and self._logger._status:
             self._logger.error(
-                f"Request DELETE guilds/{guild_id}/members/{user_id} failed.\n -> {self} {await response.json()}")
+                f"Request DELETE guilds/{guild_id}/members/{user_id} failed.\n -> {self} {await response.json()}"
+            )
 
         return response
 
     async def get_member(self, guild_id: int, user_id: int) -> ClientResponse:
         """
         The get_member function is used to get a member from the guild.
 
@@ -531,27 +578,32 @@
 
         _url = self._endpoint + f"guilds/{guild_id}/members/{user_id}"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: GET -> {_url}")
 
         response: ClientResponse = await self._session.request(
-            method="GET", url=_url, headers=self._auth_header)
+            method="GET", url=_url, headers=self._auth_header
+        )
 
         if response.status not in (200, 429) and self._logger._status:
             self._logger.error(
-                f"Request GET guilds/{guild_id}/members/{user_id} failed.\n -> {self} {await response.json()}")
+                f"Request GET guilds/{guild_id}/members/{user_id} failed.\n -> {self} {await response.json()}"
+            )
 
         return response
 
-    async def edit_member(self, guild_id: int, user_id: int,
-                          nickname: Optional[str] = None,
-                          add_roles: Optional[list[int]] = None,
-                          remove_roles: Optional[list[int]] = None) -> ClientResponse:
-
+    async def edit_member(
+        self,
+        guild_id: int,
+        user_id: int,
+        nickname: Optional[str] = None,
+        add_roles: Optional[list[int]] = None,
+        remove_roles: Optional[list[int]] = None,
+    ) -> ClientResponse:
         """
         The edit_member function allows you to edit a member of a guild.
 
         :param guild_id: Specify the guild that you want to edit a member in
         :param user_id: Specify the user that you want to edit
         :param nickname: Change the nickname of a user in a guild
         :param add_roles: Add roles to a user
@@ -585,100 +637,123 @@
 
         _url = self._endpoint + f"guilds/{guild_id}/members/{user_id}"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: PATCH -> {_url}")
 
         response: ClientResponse = await self._session.request(
-            method="PATCH", url=_url, headers=self._auth_header, json=json)
+            method="PATCH", url=_url, headers=self._auth_header, json=json
+        )
 
         if response.status not in (200, 429) and self._logger._status:
             self._logger.error(
-                f"Request PATCH guilds/{guild_id}/members/{user_id} failed.\n -> {self} {await response.json()}")
+                f"Request PATCH guilds/{guild_id}/members/{user_id} failed.\n -> {self} {await response.json()}"
+            )
 
         return response
 
-    async def add_reaction(self, channel_id: int, message_id: int, emoji: str) -> ClientResponse:
+    async def add_reaction(
+        self, channel_id: int, message_id: int, emoji: str
+    ) -> ClientResponse:
         """
         The add_reaction function adds a reaction to the message with the given ID in the channel with
         the given ID. The emoji parameter is a string that must be an emoticon. Example: \N{FIRE}
 
         :param channel_id: Specify which channel_id the message is in
         :param message_id: Message ID that you want to add a reaction to
         :param emoji: A reaction to add to the message
         """
 
         emoji = quote(emoji)
 
-        _url = self._endpoint + f"channels/{channel_id}/messages/{message_id}/reactions/{emoji}/@me"
+        _url = (
+            self._endpoint
+            + f"channels/{channel_id}/messages/{message_id}/reactions/{emoji}/@me"
+        )
 
         if self._logger._status:
             self._logger.debug(f"Sending request: PUT -> {_url}")
 
         response: ClientResponse = await self._session.request(
-            method="PUT", url=_url, headers=self._auth_header)
+            method="PUT", url=_url, headers=self._auth_header
+        )
 
         if response.status not in (204, 429) and self._logger._status:
             self._logger.error(
                 f"Request PUT channels/{channel_id}/messages/{message_id}/reactions/{emoji}/@me failed."
-                f"\n -> {self} {await response.json()}")
+                f"\n -> {self} {await response.json()}"
+            )
 
         return response
 
-    async def get_reactions(self, channel_id: int, message_id: int, emoji: str) -> ClientResponse:
+    async def get_reactions(
+        self, channel_id: int, message_id: int, emoji: str
+    ) -> ClientResponse:
         """
         The get_reactions function returns a ClientResponse with
         list of users that reacted with the specified emoji.
 
         :param channel_id: Identify the channel that contains the message
         :param message_id: Identify the message that is being reacted to
         :param emoji: Specify the emoji to get reactions for
         """
 
         emoji = quote(emoji)
 
-        _url = self._endpoint + f"channels/{channel_id}/messages/{message_id}/reactions/{emoji}"
+        _url = (
+            self._endpoint
+            + f"channels/{channel_id}/messages/{message_id}/reactions/{emoji}"
+        )
 
         if self._logger._status:
             self._logger.debug(f"Sending request: GET -> {_url}")
 
         response: ClientResponse = await self._session.request(
-            method="GET", url=_url, headers=self._auth_header)
+            method="GET", url=_url, headers=self._auth_header
+        )
 
         if response.status not in (200, 429) and self._logger._status:
             self._logger.error(
                 f"Request GET channels/{channel_id}/messages/{message_id}/reactions/{emoji}/ failed."
-                f"\n -> {self} {await response.json()}")
+                f"\n -> {self} {await response.json()}"
+            )
 
         return response
 
-    async def delete_reaction(self, channel_id: int, message_id: int, user_id: int, emoji: str) -> ClientResponse:
+    async def delete_reaction(
+        self, channel_id: int, message_id: int, user_id: int, emoji: str
+    ) -> ClientResponse:
         """
         The delete_reaction function is used to delete a reaction from a message.
 
         :param channel_id: Specify the channel where the message is located
         :param message_id: Identify the message that you want to delete a reaction from
         :param user_id: Specify the user whose reaction is to be deleted
         :param emoji: Specify the emoji to be deleted
         """
 
         emoji = quote(emoji)
 
-        _url = self._endpoint + f"channels/{channel_id}/messages/{message_id}/reactions/{emoji}/{user_id}"
+        _url = (
+            self._endpoint
+            + f"channels/{channel_id}/messages/{message_id}/reactions/{emoji}/{user_id}"
+        )
 
         if self._logger._status:
             self._logger.debug(f"Sending request: DELETE -> {_url}")
 
         response: ClientResponse = await self._session.request(
-            method="DELETE", url=_url, headers=self._auth_header)
+            method="DELETE", url=_url, headers=self._auth_header
+        )
 
         if response.status not in (204, 429) and self._logger._status:
             self._logger.error(
                 f"Request DELETE channels/{channel_id}/messages/{message_id}/reactions/{emoji}/{user_id} failed."
-                f"\n -> {self} {await response.json()}")
+                f"\n -> {self} {await response.json()}"
+            )
 
         return response
 
     async def get_guild_invites(self, guild_id: int) -> ClientResponse:
         """
         The get_guild_invites function returns a list of invite objects. Requires the 'MANAGE_GUILD' permission.
 
@@ -687,19 +762,21 @@
 
         _url = self._endpoint + f"guilds/{guild_id}/invites"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: GET -> {_url}")
 
         response: ClientResponse = await self._session.request(
-            method="GET", url=_url, headers=self._auth_header)
+            method="GET", url=_url, headers=self._auth_header
+        )
 
         if response.status not in (204, 429) and self._logger._status:
             self._logger.error(
-                f"Request GET guilds/{guild_id}/invites failed.\n -> {self} {await response.json()}")
+                f"Request GET guilds/{guild_id}/invites failed.\n -> {self} {await response.json()}"
+            )
         return response
 
     async def get_guild(self, guild_id: int) -> ClientResponse:
         """
         The get_guild function is used to get information about a guild.
 
         :param guild_id: Specify the id of the guild you want to get information about
@@ -707,63 +784,68 @@
 
         _url = self._endpoint + f"guilds/{guild_id}"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: GET -> {_url}")
 
         response: ClientResponse = await self._session.request(
-            method="GET", url=_url, headers=self._auth_header)
+            method="GET", url=_url, headers=self._auth_header
+        )
 
         if response.status not in (200, 429) and self._logger._status:
             self._logger.error(
-                f"Request GET guilds/{guild_id}/invites failed.\n -> {self} {await response.json()}")
+                f"Request GET guilds/{guild_id}/invites failed.\n -> {self} {await response.json()}"
+            )
 
         else:
             self.cache.add_guild_to_cache(await response.json())
 
         return response
 
-    async def send_dm_message(self, user_id: int, message_content: str) -> Optional[ClientResponse]:
+    async def send_dm_message(
+        self, user_id: int, message_content: str
+    ) -> Optional[ClientResponse]:
         """
         The send_dm_message function sends a direct message to the user with the given user_id.
 
         :param user_id: Specify the user id of the recipient
         :param message_content: Specify message content
         """
 
         _url = self._endpoint + "users/@me/channels"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: POST -> {_url}")
 
-        payload: dict = {
-            "recipient_id": user_id
-        }
+        payload: dict = {"recipient_id": user_id}
 
         response: ClientResponse = await self._session.request(
-            method="POST", url=_url, headers=self._auth_header, json=payload)
+            method="POST", url=_url, headers=self._auth_header, json=payload
+        )
 
         if response.status not in (200, 429) and self._logger._status:
             self._logger.error(
-                f"Request POST users/@me/channels failed.\n -> {self} {await response.json()}")
+                f"Request POST users/@me/channels failed.\n -> {self} {await response.json()}"
+            )
 
         if not response:
             return response
 
         dm_data: dict = await response.json()
         dm_channel_id: int = dm_data["id"]
 
         response: ClientResponse = await self.send_message(
-            channel_id=dm_channel_id,
-            message_content=message_content
+            channel_id=dm_channel_id, message_content=message_content
         )
 
         return response
 
-    async def __send_members_requests(self, guild_id: int, channel_id: int, limit: Optional[int]):
+    async def __send_members_requests(
+        self, guild_id: int, channel_id: int, limit: Optional[int]
+    ):
         """
         The send_members_requests function is a function that sends requests to the gateway for members.
         This function is used in the get_guild_members wrapper, and it's purpose is to send multiple requests at once.
         The reason why this function exists, and why it's not just part of get_guild_members wrapper,
         is because we want to be able to use this functionality elsewhere.
 
         :param guild_id: Get the guild id
@@ -789,30 +871,35 @@
             gateway_payload: dict = {
                 "op": 14,
                 "d": {
                     "guild_id": guild_id,
                     "typing": True,
                     "threads": False,
                     "activites": True,
-                    "channels": {channel_id: ranges_list}
-                }
+                    "channels": {channel_id: ranges_list},
+                },
             }
             if not self.gateway_connection:
-                from .gateway.errors import GatewayNotConnected
-                raise GatewayNotConnected(f"{self} does not have a gateway connection. "
-                                          f"This function only works if you run the gateway.")
+                raise GatewayNotConnected(
+                    f"{self} does not have a gateway connection. "
+                    f"This function only works if you run the gateway."
+                )
 
             gateway: GatewayConnection = self.gateway_connection
 
-            await gateway.application_update_request(request=gateway_payload,
-                                                     func=self._get_guild_members_wrapper, limit=limit)
+            await gateway.application_update_request(
+                request=gateway_payload,
+                func=self._get_guild_members_wrapper,
+                limit=limit,
+            )
             await sleep(0.6)
 
-    async def get_guild_members(self, guild_id: int, channel_id: int, limit: Optional[int] = None) \
-            -> list[Optional[dict]]:
+    async def get_guild_members(
+        self, guild_id: int, channel_id: int, limit: Optional[int] = None
+    ) -> list[Optional[dict]]:
         """
         This function doesn't quite work the same as the others.
         It uses a non-official request through the gateway by which the result may not be complete.
 
         :param guild_id: Specify the guild_id
         :param channel_id: Specify the channel from which I should fetch members
         :param limit: Provide limit of members
@@ -831,15 +918,17 @@
 
         data = self._members_data
         self._members_data = []
         self._members_end = False
 
         return data[0:limit] if limit else data
 
-    async def _get_guild_members_wrapper(self, resp_data: dict, limit: Optional[int]) -> None:
+    async def _get_guild_members_wrapper(
+        self, resp_data: dict, limit: Optional[int]
+    ) -> None:
         data: list[dict] = resp_data["ops"]
         members_data: list[Optional[dict]] = []
 
         for items_data in data:
             if not items_data["items"]:
                 self._members_end = False
             for member_data in items_data["items"]:
```

### Comparing `asynccore-1.2.0/asynccore.egg-info/SOURCES.txt` & `asynccore-1.2.1/asynccore.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 setup.py
 asynccore/__init__.py
 asynccore/__main__.py
 asynccore/activity.py
 asynccore/cache.py
```

### Comparing `asynccore-1.2.0/pyproject.toml` & `asynccore-1.2.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -10,19 +10,27 @@
 
 [tool.pylint]
 good-names="os, id, op, r, g, b"
 
 [tool.pylint.messages_control]
 max-attributes = 15
 max-args = 10
+max-branches = 13
 max-public-methods = 50
 max-locals = 30
 max-line-length=120
 disable = """
 logging-fstring-interpolation,
 missing-module-docstring,
 missing-class-docstring,
 too-few-public-methods,
 protected-access,
 missing-function-docstring,
-no-name-in-module
-"""
+no-name-in-module,
+inconsistent-return-statements
+"""
+
+[tool.ruff]
+line-length = 120
+
+[tool.ruff.per-file-ignores]
+"typings.py" = ["F401"]
```

