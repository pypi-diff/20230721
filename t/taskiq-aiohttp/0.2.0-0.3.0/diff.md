# Comparing `tmp/taskiq_aiohttp-0.2.0.tar.gz` & `tmp/taskiq_aiohttp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_aiohttp-0.2.0.tar", max compression
+gzip compressed data, was "taskiq_aiohttp-0.3.0.tar", max compression
```

## Comparing `taskiq_aiohttp-0.2.0.tar` & `taskiq_aiohttp-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-06-11 13:34:07.793958 taskiq_aiohttp-0.2.0/LICENSE
--rw-r--r--   0        0        0     2780 2023-06-11 13:34:07.793958 taskiq_aiohttp-0.2.0/README.md
--rw-r--r--   0        0        0     1713 2023-06-11 13:34:07.793958 taskiq_aiohttp-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      144 2023-06-11 13:34:07.793958 taskiq_aiohttp-0.2.0/taskiq_aiohttp/__init__.py
--rw-r--r--   0        0        0     4469 2023-06-11 13:34:07.793958 taskiq_aiohttp-0.2.0/taskiq_aiohttp/initializer.py
--rw-r--r--   0        0        0        0 2023-06-11 13:34:07.793958 taskiq_aiohttp-0.2.0/taskiq_aiohttp/py.typed
--rw-r--r--   0        0        0     3803 1970-01-01 00:00:00.000000 taskiq_aiohttp-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-21 18:35:19.923764 taskiq_aiohttp-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2780 2023-07-21 18:35:19.923764 taskiq_aiohttp-0.3.0/README.md
+-rw-r--r--   0        0        0     1721 2023-07-21 18:35:19.923764 taskiq_aiohttp-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      144 2023-07-21 18:35:19.923764 taskiq_aiohttp-0.3.0/taskiq_aiohttp/__init__.py
+-rw-r--r--   0        0        0     4553 2023-07-21 18:35:19.923764 taskiq_aiohttp-0.3.0/taskiq_aiohttp/initializer.py
+-rw-r--r--   0        0        0        0 2023-07-21 18:35:19.923764 taskiq_aiohttp-0.3.0/taskiq_aiohttp/py.typed
+-rw-r--r--   0        0        0     3807 1970-01-01 00:00:00.000000 taskiq_aiohttp-0.3.0/PKG-INFO
```

### Comparing `taskiq_aiohttp-0.2.0/LICENSE` & `taskiq_aiohttp-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq_aiohttp-0.2.0/README.md` & `taskiq_aiohttp-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `taskiq_aiohttp-0.2.0/pyproject.toml` & `taskiq_aiohttp-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "taskiq-aiohttp"
 description = "Taskiq integration with AioHTTP framework"
 authors = ["Taskiq team <taskiq@no-reply.com>"]
 maintainers = ["Taskiq team <taskiq@no-reply.com>"]
-version = "0.2.0"
+version = "0.3.0"
 readme = "README.md"
 license = "LICENSE"
 classifiers = [
     "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -21,15 +21,15 @@
     "Development Status :: 3 - Alpha",
 ]
 keywords = ["taskiq", "tasks", "distributed", "async"]
 packages = [{ include = "taskiq_aiohttp" }]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-taskiq = "^0"
+taskiq = "^0,>=0.8.0"
 aiohttp = "^3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 flake8 = "^6"
 isort = "^5.10.1"
 mypy = "^0.971"
```

### Comparing `taskiq_aiohttp-0.2.0/taskiq_aiohttp/initializer.py` & `taskiq_aiohttp-0.3.0/taskiq_aiohttp/initializer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 import inspect
-from typing import Any, Awaitable, Callable
+from typing import Awaitable, Callable
 
 import yarl
 from aiohttp import web
 from aiohttp.http_writer import HttpVersion10
 from aiohttp.web_protocol import RequestHandler
 from aiohttp.web_request import RawRequestMessage
 from aiohttp.web_urldispatcher import SystemRoute, UrlMappingMatchInfo
@@ -67,100 +67,103 @@
         {
             web.Application: app,
             web.Request: request,
         },
     )
 
 
-def startup_event_generator(
+def startup_event_generator(  # noqa: C901
     broker: AsyncBroker,
     app_path: str,
-    app: Any,
 ) -> Callable[[TaskiqState], Awaitable[None]]:
     """
     Creates an event to run on broker's startup.
 
     This function create a mock application for
     later use and updates broker's dependency context.
 
     Also we run application's startup event so it would
     act the same as the real application.
 
     :param broker: current broker.
     :param app_path: path to the application.
-    :param app: current application or a fractory.
 
     :returns: a function that is called on startup.
     """
 
     async def startup(state: TaskiqState) -> None:
-        local_app = app
+        if not broker.is_worker_process:
+            return
 
-        if not isinstance(local_app, web.Application):
-            local_app = local_app()
+        app = import_object(app_path)
 
-        if inspect.iscoroutine(local_app):
-            local_app = await local_app
-        if not isinstance(local_app, web.Application):
+        if not isinstance(app, web.Application):
+            app = app()
+
+        if inspect.iscoroutine(app):
+            app = await app
+        if not isinstance(app, web.Application):
             raise ValueError(f"{app_path} is not an AioHTTP application.")
 
         # Starting the application.
-        app_runner = web.AppRunner(local_app)
+        app_runner = web.AppRunner(app)
         await app_runner.setup()
 
         if app_runner.server is None:
             raise ValueError("Cannot construct aiohttp app to mock requests")
 
         loop = asyncio.get_running_loop()
 
         populate_context(
             broker=broker,
             server=app_runner.server,
-            app=local_app,
+            app=app,
             loop=loop,
         )
 
         # Creating mocked request
         state.aiohttp_runner = app_runner
-        local_app.router._resources = []
+        app.router._resources = []
 
     return startup
 
 
-async def shutdown(state: TaskiqState) -> None:
+def shutdown_generator(broker: AsyncBroker) -> Callable[[TaskiqState], Awaitable[None]]:
     """
-    Shuts down the app.
+    Shuts down event generator.
 
-    It just gets the application
-    we created in startup and shuts it down.
+    This function generates a shutdown broker
 
-    :param state: current state.
+    :param broker: current broker.
+    :returns: shutdown event handler.
     """
-    await state.aiohttp_runner.shutdown()
-    await state.aiohttp_runner.cleanup()
+
+    async def shutdown(state: TaskiqState) -> None:
+        if not broker.is_worker_process:
+            return
+
+        await state.aiohttp_runner.shutdown()
+        await state.aiohttp_runner.cleanup()
+
+    return shutdown
 
 
 def init(broker: AsyncBroker, app_path: str) -> None:
     """
     Initialize dependencies for your taskiq.
 
     This function imports your application and tries to
     update broker's dependency context, so request and
     applicaiton will be available in all your taskiq
     dependencies.
 
     :param broker: current broker.
     :param app_path: string with a path to an application or a factory.
     """
-    if not broker.is_worker_process:
-        return
-
-    app = import_object(app_path)
-
     broker.add_event_handler(
         TaskiqEvents.WORKER_STARTUP,
-        startup_event_generator(broker, app_path, app),
+        startup_event_generator(broker, app_path),
     )
     broker.add_event_handler(
         TaskiqEvents.WORKER_SHUTDOWN,
-        shutdown,
+        shutdown_generator(broker),
     )
```

### Comparing `taskiq_aiohttp-0.2.0/PKG-INFO` & `taskiq_aiohttp-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq-aiohttp
-Version: 0.2.0
+Version: 0.3.0
 Summary: Taskiq integration with AioHTTP framework
 License: LICENSE
 Keywords: taskiq,tasks,distributed,async
 Author: Taskiq team
 Author-email: taskiq@no-reply.com
 Maintainer: Taskiq team
 Maintainer-email: taskiq@no-reply.com
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: System :: Networking
 Classifier: Typing :: Typed
 Requires-Dist: aiohttp (>=3,<4)
-Requires-Dist: taskiq (>=0,<1)
+Requires-Dist: taskiq (>=0.8.0,<1)
 Description-Content-Type: text/markdown
 
 # Taskiq + AioHTTP
 
 This project is used to create mocked application and request
 that you can use as a dependencies in your taskiq application.
```

