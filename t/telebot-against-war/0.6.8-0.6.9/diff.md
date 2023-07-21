# Comparing `tmp/telebot_against_war-0.6.8.tar.gz` & `tmp/telebot_against_war-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telebot_against_war-0.6.8.tar", max compression
+gzip compressed data, was "telebot_against_war-0.6.9.tar", max compression
```

## Comparing `telebot_against_war-0.6.8.tar` & `telebot_against_war-0.6.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    18047 2023-07-12 08:53:22.207892 telebot_against_war-0.6.8/LICENSE
--rw-r--r--   0        0        0     2064 2023-07-12 08:53:22.211892 telebot_against_war-0.6.8/README.md
--rw-r--r--   0        0        0     1103 2023-07-12 08:53:42.500264 telebot_against_war-0.6.8/pyproject.toml
--rw-r--r--   0        0        0   157511 2023-07-12 08:53:22.211892 telebot_against_war-0.6.8/telebot/__init__.py
--rw-r--r--   0        0        0    82566 2023-07-12 08:53:22.211892 telebot_against_war-0.6.8/telebot/api.py
--rw-r--r--   0        0        0     5034 2023-07-12 08:53:22.211892 telebot_against_war-0.6.8/telebot/callback_data.py
--rw-r--r--   0        0        0     2913 2023-07-12 08:53:22.211892 telebot_against_war-0.6.8/telebot/check_text.py
--rw-r--r--   0        0        0     4733 2023-07-12 08:53:22.211892 telebot_against_war-0.6.8/telebot/filters.py
--rw-r--r--   0        0        0     8645 2023-07-12 08:53:22.211892 telebot_against_war-0.6.8/telebot/formatting.py
--rw-r--r--   0        0        0     3225 2023-07-12 08:53:22.211892 telebot_against_war-0.6.8/telebot/graceful_shutdown.py
--rw-r--r--   0        0        0     2049 2023-07-12 08:53:22.211892 telebot_against_war-0.6.8/telebot/helpers.py
--rw-r--r--   0        0        0     2046 2023-07-12 08:53:22.211892 telebot_against_war-0.6.8/telebot/metrics.py
--rw-r--r--   0        0        0        0 2023-07-12 08:53:22.211892 telebot_against_war-0.6.8/telebot/py.typed
--rw-r--r--   0        0        0     1797 2023-07-12 08:53:22.211892 telebot_against_war-0.6.8/telebot/runner.py
--rw-r--r--   0        0        0      396 2023-07-12 08:53:22.211892 telebot_against_war-0.6.8/telebot/storages/__init__.py
--rw-r--r--   0        0        0     1710 2023-07-12 08:53:22.211892 telebot_against_war-0.6.8/telebot/storages/base_storage.py
--rw-r--r--   0        0        0     2296 2023-07-12 08:53:22.211892 telebot_against_war-0.6.8/telebot/storages/memory_storage.py
--rw-r--r--   0        0        0     3695 2023-07-12 08:53:22.211892 telebot_against_war-0.6.8/telebot/storages/pickle_storage.py
--rw-r--r--   0        0        0     5626 2023-07-12 08:53:22.211892 telebot_against_war-0.6.8/telebot/storages/redis_storage.py
--rw-r--r--   0        0        0    35492 2023-07-12 08:53:22.211892 telebot_against_war-0.6.8/telebot/test_util.py
--rw-r--r--   0        0        0   157020 2023-07-12 08:53:22.215892 telebot_against_war-0.6.8/telebot/types/__init__.py
--rw-r--r--   0        0        0     2724 2023-07-12 08:53:22.215892 telebot_against_war-0.6.8/telebot/types/constants.py
--rw-r--r--   0        0        0     1885 2023-07-12 08:53:22.215892 telebot_against_war-0.6.8/telebot/types/service.py
--rw-r--r--   0        0        0    10649 2023-07-12 08:53:22.215892 telebot_against_war-0.6.8/telebot/util.py
--rw-r--r--   0        0        0     8424 2023-07-12 08:53:22.215892 telebot_against_war-0.6.8/telebot/webhook.py
--rw-r--r--   0        0        0     2851 1970-01-01 00:00:00.000000 telebot_against_war-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0    18047 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/LICENSE
+-rw-r--r--   0        0        0     2064 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/README.md
+-rw-r--r--   0        0        0     1103 2023-07-21 12:46:56.218373 telebot_against_war-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0   157511 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/__init__.py
+-rw-r--r--   0        0        0    82566 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/api.py
+-rw-r--r--   0        0        0     5034 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/callback_data.py
+-rw-r--r--   0        0        0     2913 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/check_text.py
+-rw-r--r--   0        0        0     4733 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/filters.py
+-rw-r--r--   0        0        0     8645 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/formatting.py
+-rw-r--r--   0        0        0     3225 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/graceful_shutdown.py
+-rw-r--r--   0        0        0     2049 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/helpers.py
+-rw-r--r--   0        0        0     2046 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/metrics.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/py.typed
+-rw-r--r--   0        0        0     1797 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/runner.py
+-rw-r--r--   0        0        0      396 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/storages/__init__.py
+-rw-r--r--   0        0        0     1710 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/storages/base_storage.py
+-rw-r--r--   0        0        0     2296 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/storages/memory_storage.py
+-rw-r--r--   0        0        0     3695 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/storages/pickle_storage.py
+-rw-r--r--   0        0        0     5626 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/storages/redis_storage.py
+-rw-r--r--   0        0        0    35492 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/test_util.py
+-rw-r--r--   0        0        0   157020 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/types/__init__.py
+-rw-r--r--   0        0        0     2724 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/types/constants.py
+-rw-r--r--   0        0        0     1885 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/types/service.py
+-rw-r--r--   0        0        0    10649 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/util.py
+-rw-r--r--   0        0        0     8685 2023-07-21 12:46:38.210431 telebot_against_war-0.6.9/telebot/webhook.py
+-rw-r--r--   0        0        0     2851 1970-01-01 00:00:00.000000 telebot_against_war-0.6.9/PKG-INFO
```

### Comparing `telebot_against_war-0.6.8/LICENSE` & `telebot_against_war-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.8/README.md` & `telebot_against_war-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.8/pyproject.toml` & `telebot_against_war-0.6.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "telebot-against-war"
-version = "0.6.8"  # replaced by dynamic versioning plugin
+version = "0.6.9"  # replaced by dynamic versioning plugin
 description = "Async-first fork of pyTelegramBotApi"
 authors = ["Igor Vaiman <gosha.vaiman@gmail.com>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 repository = "https://github.com/bots-against-war/telebot"
 packages = [
     { include = "telebot" },
```

### Comparing `telebot_against_war-0.6.8/telebot/__init__.py` & `telebot_against_war-0.6.9/telebot/__init__.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.8/telebot/api.py` & `telebot_against_war-0.6.9/telebot/api.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.8/telebot/callback_data.py` & `telebot_against_war-0.6.9/telebot/callback_data.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.8/telebot/check_text.py` & `telebot_against_war-0.6.9/telebot/check_text.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.8/telebot/filters.py` & `telebot_against_war-0.6.9/telebot/filters.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.8/telebot/formatting.py` & `telebot_against_war-0.6.9/telebot/formatting.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.8/telebot/graceful_shutdown.py` & `telebot_against_war-0.6.9/telebot/graceful_shutdown.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.8/telebot/helpers.py` & `telebot_against_war-0.6.9/telebot/helpers.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.8/telebot/metrics.py` & `telebot_against_war-0.6.9/telebot/metrics.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.8/telebot/runner.py` & `telebot_against_war-0.6.9/telebot/runner.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.8/telebot/storages/base_storage.py` & `telebot_against_war-0.6.9/telebot/storages/base_storage.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.8/telebot/storages/memory_storage.py` & `telebot_against_war-0.6.9/telebot/storages/memory_storage.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.8/telebot/storages/pickle_storage.py` & `telebot_against_war-0.6.9/telebot/storages/pickle_storage.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.8/telebot/storages/redis_storage.py` & `telebot_against_war-0.6.9/telebot/storages/redis_storage.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.8/telebot/test_util.py` & `telebot_against_war-0.6.9/telebot/test_util.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.8/telebot/types/__init__.py` & `telebot_against_war-0.6.9/telebot/types/__init__.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.8/telebot/types/constants.py` & `telebot_against_war-0.6.9/telebot/types/constants.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.8/telebot/types/service.py` & `telebot_against_war-0.6.9/telebot/types/service.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.8/telebot/util.py` & `telebot_against_war-0.6.9/telebot/util.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.8/telebot/webhook.py` & `telebot_against_war-0.6.9/telebot/webhook.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import collections
 import logging
 import signal
 import time
 from types import FrameType
 from typing import Any, Awaitable, Callable, Coroutine, Optional
 
 from aiohttp import web
@@ -28,21 +29,20 @@
     def __init__(
         self,
         base_url: str,
         metrics_handler: Callable[[TelegramUpdateMetrics], Awaitable[None]] = noop_metrics_handler,
     ):
         self.base_url = base_url
         self.bot_runner_by_subroute: dict[str, BotRunner] = dict()
-        self.background_tasks: set[asyncio.Task] = set()
+        self.background_task_by_bot_subroute: dict[str, set[asyncio.Task]] = collections.defaultdict(set)
         self.aiohttp_app = web.Application()
         self.aiohttp_app.router.add_post(WEBHOOK_ROUTE, self._bot_webhook_handler)
         self.aiohttp_app.middlewares.append(self._graceful_shutdown_middleware)
         self._current_request_count = 0
         self._is_shutting_down = False
-        self._is_cleaning_up = False
         self._metrics_handler = metrics_handler
 
     async def _bot_webhook_handler(self, request: web.Request):
         subroute = request.match_info.get("subroute")
         if subroute is None:
             return web.Response(status=404)
         bot_runner = self.bot_runner_by_subroute.get(subroute)
@@ -104,14 +104,17 @@
                     break
             else:
                 logger.info("All shutdown conditions are satisfied, shutting down")
                 raise SystemExit()
 
     async def add_bot_runner(self, runner: BotRunner) -> bool:
         subroute = runner.webhook_subroute()
+        if subroute in self.bot_runner_by_subroute:
+            logger.info("Attempt to set bot runner for already existing subroute")
+            return False
         webhook_url = self.base_url + WEBHOOK_ROUTE.format(subroute=subroute)
         try:
             existing_webhook_info = await runner.bot.get_webhook_info()
             if existing_webhook_info.url == webhook_url:
                 logger.info(f"Existing webhook found for {runner.bot_prefix}")
             else:
                 await runner.bot.set_webhook(url=webhook_url)
@@ -127,46 +130,55 @@
                 endpoint.handler,
             )
             logger.info(f"Aux endpoint created for {runner.bot_prefix}: {endpoint.route}")
 
         for idx, coro in enumerate(runner.background_jobs):
             idx += 1  # 1-based numbering
             task = create_error_logging_task(coro, name=f"{runner.bot_prefix}-{idx}")
-            self.background_tasks.add(task)
+            self.background_task_by_bot_subroute[subroute].add(task)
 
             def background_job_done(task: asyncio.Task):
-                if not self._is_cleaning_up:
-                    # during cleanup we iterate over background tasks set, so we can't change its size!
-                    self.background_tasks.discard(task)
                 if task.cancelled():
                     logger.info(f"Backgound job cancelled: {task}")
                 else:
                     logger.info(f"Backgound job completed: {task}")
 
             task.add_done_callback(background_job_done)
             logger.info(f"Background task created for {runner.bot_prefix} ({idx}/{len(runner.background_jobs)})")
 
         self.bot_runner_by_subroute[subroute] = runner
         return True
 
     async def remove_bot_runner(self, runner: BotRunner) -> bool:
-        """Warning: background jobs and aux endpoints added with the runner are not removed/cancelled"""
         subroute = runner.webhook_subroute()
         if subroute not in self.bot_runner_by_subroute:
             return False
         try:
             await runner.bot.delete_webhook()
             logger.info(f"Webhook removed for {runner.bot_prefix}; was /webhook/{subroute}")
-        except Exception as e:
-            logger.exception(f"Error deleting webhook for the bot {runner.bot_prefix}, keeping it")
+        except Exception:
+            logger.exception(f"Error deleting webhook for the bot {runner.bot_prefix}")
             return False
-
+        await self._cancel_background_tasks(subroute)
+        self.background_task_by_bot_subroute.pop(subroute, None)
         self.bot_runner_by_subroute.pop(subroute)
         return True
 
+    async def _cancel_background_tasks(self, subroute: str) -> None:
+        tasks = self.background_task_by_bot_subroute.get(subroute)
+        if tasks is None:
+            return
+        for task in tasks:
+            logger.debug(f"Cancelling background task {task} for {subroute}")
+            task.cancel()
+            try:
+                await task
+            except asyncio.CancelledError:
+                pass
+
     async def run(
         self,
         port: int,
         graceful_shutdown: bool = True,
         on_server_listening: Optional[Callable[[], Coroutine[None, None, Any]]] = None,
     ):
         aiohttp_runner = web.AppRunner(self.aiohttp_app, access_log=None)
@@ -180,19 +192,14 @@
                 signal.signal(signal.SIGINT, self._graceful_shutdown_signal_handler)
                 signal.signal(signal.SIGTERM, self._graceful_shutdown_signal_handler)
                 await self._graceful_shutdown_monitor()
             else:
                 while True:
                     await asyncio.sleep(3600)
         finally:
-            self._is_cleaning_up = True
             logger.debug("Cleanup started")
+            for subroute in self.background_task_by_bot_subroute:
+                await self._cancel_background_tasks(subroute)
+
             await api.session_manager.close_session()
-            for t in self.background_tasks:
-                logger.debug(f"Cancelling background task {t}")
-                t.cancel()
-                try:
-                    await t
-                except asyncio.CancelledError:
-                    pass
-            logger.debug("Cleanup completed")
             await aiohttp_runner.cleanup()
+            logger.debug("Cleanup completed")
```

### Comparing `telebot_against_war-0.6.8/PKG-INFO` & `telebot_against_war-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telebot-against-war
-Version: 0.6.8
+Version: 0.6.9
 Summary: Async-first fork of pyTelegramBotApi
 Home-page: https://github.com/bots-against-war/telebot
 License: GPL-2.0-only
 Author: Igor Vaiman
 Author-email: gosha.vaiman@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: telebot-against-war Version: 0.6.8 Summary: Async-
+Metadata-Version: 2.1 Name: telebot-against-war Version: 0.6.9 Summary: Async-
 first fork of pyTelegramBotApi Home-page: https://github.com/bots-against-war/
 telebot License: GPL-2.0-only Author: Igor Vaiman Author-email:
 gosha.vaiman@gmail.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v2 (GPLv2) Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: aiohttp (>=3.8.1,<4.0.0) Requires-
```

