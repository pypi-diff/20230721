# Comparing `tmp/taskiq_fastapi-0.2.0.tar.gz` & `tmp/taskiq_fastapi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_fastapi-0.2.0.tar", max compression
+gzip compressed data, was "taskiq_fastapi-0.3.0.tar", max compression
```

## Comparing `taskiq_fastapi-0.2.0.tar` & `taskiq_fastapi-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1073 2023-06-11 13:20:21.216347 taskiq_fastapi-0.2.0/LICENSE
--rw-r--r--   0        0        0     4034 2023-06-11 13:20:21.216347 taskiq_fastapi-0.2.0/README.md
--rw-r--r--   0        0        0     1565 2023-06-11 13:20:21.216347 taskiq_fastapi-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      172 2023-06-11 13:20:21.216347 taskiq_fastapi-0.2.0/taskiq_fastapi/__init__.py
--rw-r--r--   0        0        0     2646 2023-06-11 13:20:21.216347 taskiq_fastapi-0.2.0/taskiq_fastapi/initializator.py
--rw-r--r--   0        0        0     5049 1970-01-01 00:00:00.000000 taskiq_fastapi-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-21 16:38:11.874874 taskiq_fastapi-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4034 2023-07-21 16:38:11.874874 taskiq_fastapi-0.3.0/README.md
+-rw-r--r--   0        0        0     1565 2023-07-21 16:38:11.874874 taskiq_fastapi-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-07-21 16:38:11.874874 taskiq_fastapi-0.3.0/taskiq_fastapi/__init__.py
+-rw-r--r--   0        0        0     2808 2023-07-21 16:38:11.874874 taskiq_fastapi-0.3.0/taskiq_fastapi/initializator.py
+-rw-r--r--   0        0        0     5049 1970-01-01 00:00:00.000000 taskiq_fastapi-0.3.0/PKG-INFO
```

### Comparing `taskiq_fastapi-0.2.0/LICENSE` & `taskiq_fastapi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq_fastapi-0.2.0/README.md` & `taskiq_fastapi-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `taskiq_fastapi-0.2.0/pyproject.toml` & `taskiq_fastapi-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "taskiq-fastapi"
 description = "FastAPI integration for taskiq"
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
 keywords = ["taskiq", "tasks", "distributed", "async", "fastapi"]
 packages = [{ include = "taskiq_fastapi" }]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-taskiq = "^0,>=0.3.1"
+taskiq = "^0,>=0.8.0"
 fastapi = "*"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6"
 isort = "^5.10.1"
 mypy = "^0.971"
 pre-commit = "^2.20.0"
```

### Comparing `taskiq_fastapi-0.2.0/taskiq_fastapi/initializator.py` & `taskiq_fastapi-0.3.0/taskiq_fastapi/initializator.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,86 +2,90 @@
 
 from fastapi import FastAPI, Request
 from starlette.requests import HTTPConnection
 from taskiq import AsyncBroker, TaskiqEvents, TaskiqState
 from taskiq.cli.utils import import_object
 
 
-def startup_event_generator(app: FastAPI) -> Callable[[TaskiqState], Awaitable[None]]:
+def startup_event_generator(
+    broker: AsyncBroker,
+    app_path: str,
+) -> Callable[[TaskiqState], Awaitable[None]]:
     """
     Generate shutdown event.
 
-    This function takes FastAPI application
+    This function takes FastAPI application path
     and runs startup event on broker's startup.
 
-    :param app: fastapi application.
+    :param broker: current broker.
+    :param app_path: fastapi application path.
     :returns: startup handler.
     """
 
     async def startup(state: TaskiqState) -> None:
+        if not broker.is_worker_process:
+            return
+        app = import_object(app_path)
+        if not isinstance(app, FastAPI):
+            app = app()
+
+        if not isinstance(app, FastAPI):
+            raise ValueError(f"'{app_path}' is not a FastAPI application.")
+
         state.fastapi_app = app
         app.router.routes = []
         await app.router.startup()
+        populate_dependency_context(broker, app)
 
     return startup
 
 
-def shutdown_event_generator(app: FastAPI) -> Callable[[TaskiqState], Awaitable[None]]:
+def shutdown_event_generator(
+    broker: AsyncBroker,
+) -> Callable[[TaskiqState], Awaitable[None]]:
     """
     Generate shutdown event.
 
     This function takes FastAPI application
     and runs shutdown event on broker's shutdown.
 
-    :param app: current application.
-    :return: startup event handler.
+    :param broker: current broker.
+    :return: shutdown event handler.
     """
 
-    async def startup(_: TaskiqState) -> None:
-        await app.router.shutdown()
+    async def shutdown(state: TaskiqState) -> None:
+        if not broker.is_worker_process:
+            return
+        await state.fastapi_app.router.shutdown()
 
-    return startup
+    return shutdown
 
 
 def init(broker: AsyncBroker, app_path: str) -> None:
     """
     Add taskiq startup events.
 
     This is the main function to integrate FastAPI
     with taskiq.
 
-    This function imports fastapi application by
-    python's path string and adds startup events
-    for broker.
+    It creates startup events for broker. So
+    in worker processes all fastapi
+    startup events will run.
 
     :param broker: current broker to use.
     :param app_path: path to fastapi application.
-    :raises ValueError: if fastapi cannot be resolved.
     """
-    if not broker.is_worker_process:
-        return
-
-    app = import_object(app_path)
-
-    if not isinstance(app, FastAPI):
-        app = app()
-
-    if not isinstance(app, FastAPI):
-        raise ValueError(f"'{app_path}' is not a FastAPI application.")
-
-    populate_dependency_context(broker, app)
-
     broker.add_event_handler(
         TaskiqEvents.WORKER_STARTUP,
-        startup_event_generator(app),
+        startup_event_generator(broker, app_path),
     )
 
     broker.add_event_handler(
         TaskiqEvents.WORKER_SHUTDOWN,
-        shutdown_event_generator(app),
+        shutdown_event_generator(broker),
     )
 
 
 def populate_dependency_context(broker: AsyncBroker, app: FastAPI) -> None:
     """
     Populate dependency context.
```

### Comparing `taskiq_fastapi-0.2.0/PKG-INFO` & `taskiq_fastapi-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq-fastapi
-Version: 0.2.0
+Version: 0.3.0
 Summary: FastAPI integration for taskiq
 License: LICENSE
 Keywords: taskiq,tasks,distributed,async,fastapi
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
 Requires-Dist: fastapi
-Requires-Dist: taskiq (>=0.3.1,<1)
+Requires-Dist: taskiq (>=0.8.0,<1)
 Description-Content-Type: text/markdown
 
 # Taskiq + FastAPI
 
 This repository has a code to integrate FastAPI with taskiq easily.
 
 Taskiq and FastAPI both have dependencies and this library makes it possible to depend on
```

