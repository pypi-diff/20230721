# Comparing `tmp/pylitterbot-2023.4.2.tar.gz` & `tmp/pylitterbot-2023.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylitterbot-2023.4.2.tar", max compression
+gzip compressed data, was "pylitterbot-2023.4.3.tar", max compression
```

## Comparing `pylitterbot-2023.4.2.tar` & `pylitterbot-2023.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1076 2023-06-08 20:14:06.723140 pylitterbot-2023.4.2/LICENSE
--rw-r--r--   0        0        0     3168 2023-06-08 20:14:06.723140 pylitterbot-2023.4.2/README.md
--rw-r--r--   0        0        0      403 2023-06-08 20:14:24.295435 pylitterbot-2023.4.2/pylitterbot/__init__.py
--rw-r--r--   0        0        0     7546 2023-06-08 20:14:06.723140 pylitterbot-2023.4.2/pylitterbot/account.py
--rw-r--r--   0        0        0     1118 2023-06-08 20:14:06.723140 pylitterbot-2023.4.2/pylitterbot/activity.py
--rw-r--r--   0        0        0     4597 2023-06-08 20:14:06.723140 pylitterbot-2023.4.2/pylitterbot/enums.py
--rw-r--r--   0        0        0      348 2023-06-08 20:14:06.723140 pylitterbot-2023.4.2/pylitterbot/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-08 20:14:06.723140 pylitterbot-2023.4.2/pylitterbot/py.typed
--rw-r--r--   0        0        0     6838 2023-06-08 20:14:06.723140 pylitterbot-2023.4.2/pylitterbot/robot/__init__.py
--rw-r--r--   0        0        0    10446 2023-06-08 20:14:06.723140 pylitterbot-2023.4.2/pylitterbot/robot/feederrobot.py
--rw-r--r--   0        0        0     7187 2023-06-08 20:14:06.723140 pylitterbot-2023.4.2/pylitterbot/robot/litterrobot.py
--rw-r--r--   0        0        0    11704 2023-06-08 20:14:06.723140 pylitterbot-2023.4.2/pylitterbot/robot/litterrobot3.py
--rw-r--r--   0        0        0    25443 2023-06-08 20:14:06.723140 pylitterbot-2023.4.2/pylitterbot/robot/litterrobot4.py
--rw-r--r--   0        0        0     2364 2023-06-08 20:14:06.723140 pylitterbot-2023.4.2/pylitterbot/robot/models.py
--rw-r--r--   0        0        0     7890 2023-06-08 20:14:06.723140 pylitterbot-2023.4.2/pylitterbot/session.py
--rw-r--r--   0        0        0     3727 2023-06-08 20:14:06.723140 pylitterbot-2023.4.2/pylitterbot/utils.py
--rw-r--r--   0        0        0     5148 2023-06-08 20:14:06.723140 pylitterbot-2023.4.2/pylitterbot/ws_monitor.py
--rw-r--r--   0        0        0     1154 2023-06-08 20:14:24.295435 pylitterbot-2023.4.2/pyproject.toml
--rw-r--r--   0        0        0     4088 1970-01-01 00:00:00.000000 pylitterbot-2023.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-21 00:36:56.162145 pylitterbot-2023.4.3/LICENSE
+-rw-r--r--   0        0        0     3168 2023-07-21 00:36:56.162145 pylitterbot-2023.4.3/README.md
+-rw-r--r--   0        0        0      403 2023-07-21 00:37:12.250360 pylitterbot-2023.4.3/pylitterbot/__init__.py
+-rw-r--r--   0        0        0     7881 2023-07-21 00:36:56.166145 pylitterbot-2023.4.3/pylitterbot/account.py
+-rw-r--r--   0        0        0     1118 2023-07-21 00:36:56.166145 pylitterbot-2023.4.3/pylitterbot/activity.py
+-rw-r--r--   0        0        0     4597 2023-07-21 00:36:56.166145 pylitterbot-2023.4.3/pylitterbot/enums.py
+-rw-r--r--   0        0        0      348 2023-07-21 00:36:56.166145 pylitterbot-2023.4.3/pylitterbot/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-21 00:36:56.166145 pylitterbot-2023.4.3/pylitterbot/py.typed
+-rw-r--r--   0        0        0     6966 2023-07-21 00:36:56.166145 pylitterbot-2023.4.3/pylitterbot/robot/__init__.py
+-rw-r--r--   0        0        0    10446 2023-07-21 00:36:56.166145 pylitterbot-2023.4.3/pylitterbot/robot/feederrobot.py
+-rw-r--r--   0        0        0     7187 2023-07-21 00:36:56.166145 pylitterbot-2023.4.3/pylitterbot/robot/litterrobot.py
+-rw-r--r--   0        0        0    11704 2023-07-21 00:36:56.166145 pylitterbot-2023.4.3/pylitterbot/robot/litterrobot3.py
+-rw-r--r--   0        0        0    25443 2023-07-21 00:36:56.166145 pylitterbot-2023.4.3/pylitterbot/robot/litterrobot4.py
+-rw-r--r--   0        0        0     2364 2023-07-21 00:36:56.166145 pylitterbot-2023.4.3/pylitterbot/robot/models.py
+-rw-r--r--   0        0        0     7890 2023-07-21 00:36:56.166145 pylitterbot-2023.4.3/pylitterbot/session.py
+-rw-r--r--   0        0        0     3727 2023-07-21 00:36:56.166145 pylitterbot-2023.4.3/pylitterbot/utils.py
+-rw-r--r--   0        0        0     5148 2023-07-21 00:36:56.166145 pylitterbot-2023.4.3/pylitterbot/ws_monitor.py
+-rw-r--r--   0        0        0     1154 2023-07-21 00:37:12.250360 pylitterbot-2023.4.3/pyproject.toml
+-rw-r--r--   0        0        0     4088 1970-01-01 00:00:00.000000 pylitterbot-2023.4.3/PKG-INFO
```

### Comparing `pylitterbot-2023.4.2/LICENSE` & `pylitterbot-2023.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.2/README.md` & `pylitterbot-2023.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.2/pylitterbot/account.py` & `pylitterbot-2023.4.3/pylitterbot/account.py`

 * *Files 6% similar despite different names*

```diff
@@ -138,14 +138,21 @@
             ]
             resp = await asyncio.gather(*all_robots)
 
             async def update_or_create_robot(
                 robot_cls: type[Robot], data: dict
             ) -> None:
                 # pylint: disable=protected-access
+                if data.get(robot_cls._data_serial) is None:
+                    _LOGGER.info(
+                        "skipping robot without serial number (id=%s, name=%s)",
+                        data.get(robot_cls._data_id),
+                        data.get(robot_cls._data_name),
+                    )
+                    return
                 if robot := self.get_robot(data.get(robot_cls._data_id)):
                     robot._update_data(data)
                 else:
                     robot = robot_cls(data=data, account=self)
                     if subscribe_for_updates:
                         await robot.subscribe()
                 robots.append(robot)
```

### Comparing `pylitterbot-2023.4.2/pylitterbot/activity.py` & `pylitterbot-2023.4.3/pylitterbot/activity.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.2/pylitterbot/enums.py` & `pylitterbot-2023.4.3/pylitterbot/enums.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.2/pylitterbot/robot/__init__.py` & `pylitterbot-2023.4.3/pylitterbot/robot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,16 @@
         self._is_loaded = False
         self._listeners: dict[str, list[Callable]] = {}
 
         self._ws: ClientWebSocketResponse | None = None
         self._ws_subscription_id: str | None = None
 
         if data:
+            if data.get(self._data_serial) is None:
+                raise ValueError("Robot data must include a serial number")
             self._update_data(data)
 
     def __str__(self) -> str:
         """Return str(self)."""
         return f"Name: {self.name}, Model: {self.model}, Serial: {self.serial}, id: {self.id}"
 
     @property
```

### Comparing `pylitterbot-2023.4.2/pylitterbot/robot/feederrobot.py` & `pylitterbot-2023.4.3/pylitterbot/robot/feederrobot.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.2/pylitterbot/robot/litterrobot.py` & `pylitterbot-2023.4.3/pylitterbot/robot/litterrobot.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.2/pylitterbot/robot/litterrobot3.py` & `pylitterbot-2023.4.3/pylitterbot/robot/litterrobot3.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.2/pylitterbot/robot/litterrobot4.py` & `pylitterbot-2023.4.3/pylitterbot/robot/litterrobot4.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.2/pylitterbot/robot/models.py` & `pylitterbot-2023.4.3/pylitterbot/robot/models.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.2/pylitterbot/session.py` & `pylitterbot-2023.4.3/pylitterbot/session.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.2/pylitterbot/utils.py` & `pylitterbot-2023.4.3/pylitterbot/utils.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.2/pylitterbot/ws_monitor.py` & `pylitterbot-2023.4.3/pylitterbot/ws_monitor.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.2/pyproject.toml` & `pylitterbot-2023.4.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylitterbot"
-version = "2023.4.2"
+version = "2023.4.3"
 description = "Python package for controlling Whisker automatic robots."
 authors = ["Nathan Spencer <natekspencer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/natekspencer/pylitterbot"
 repository = "https://github.com/natekspencer/pylitterbot"
 keywords = ["Whisker", "Litter-Robot", "Feeder-Robot", "litter box", "pet feeder", "asynchronous"]
```

### Comparing `pylitterbot-2023.4.2/PKG-INFO` & `pylitterbot-2023.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylitterbot
-Version: 2023.4.2
+Version: 2023.4.3
 Summary: Python package for controlling Whisker automatic robots.
 Home-page: https://github.com/natekspencer/pylitterbot
 License: MIT
 Keywords: Whisker,Litter-Robot,Feeder-Robot,litter box,pet feeder,asynchronous
 Author: Nathan Spencer
 Author-email: natekspencer@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

