# Comparing `tmp/taskiq-0.8.4.tar.gz` & `tmp/taskiq-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq-0.8.4.tar", max compression
+gzip compressed data, was "taskiq-0.8.5.tar", max compression
```

## Comparing `taskiq-0.8.4.tar` & `taskiq-0.8.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     1075 2023-07-18 20:22:04.741682 taskiq-0.8.4/LICENSE
--rw-r--r--   0        0        0     1875 2023-07-18 20:22:04.741682 taskiq-0.8.4/README.md
--rw-r--r--   0        0        0     3007 2023-07-18 20:22:04.745682 taskiq-0.8.4/pyproject.toml
--rw-r--r--   0        0        0     2022 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/__init__.py
--rw-r--r--   0        0        0     2093 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/__main__.py
--rw-r--r--   0        0        0      194 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/abc/__init__.py
--rw-r--r--   0        0        0    12959 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/abc/broker.py
--rw-r--r--   0        0        0      323 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/abc/cmd.py
--rw-r--r--   0        0        0      629 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/abc/formatter.py
--rw-r--r--   0        0        0     3562 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/abc/middleware.py
--rw-r--r--   0        0        0     1376 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/abc/result_backend.py
--rw-r--r--   0        0        0     1623 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/abc/schedule_source.py
--rw-r--r--   0        0        0      496 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/acks.py
--rw-r--r--   0        0        0       34 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/brokers/__init__.py
--rw-r--r--   0        0        0     5679 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/brokers/inmemory_broker.py
--rw-r--r--   0        0        0     2197 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/brokers/shared_broker.py
--rw-r--r--   0        0        0     2831 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/brokers/zmq_broker.py
--rw-r--r--   0        0        0       31 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/cli/__init__.py
--rw-r--r--   0        0        0      197 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/cli/common_args.py
--rw-r--r--   0        0        0       37 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/cli/scheduler/__init__.py
--rw-r--r--   0        0        0     2076 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/cli/scheduler/args.py
--rw-r--r--   0        0        0      651 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/cli/scheduler/cmd.py
--rw-r--r--   0        0        0     3767 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/cli/scheduler/run.py
--rw-r--r--   0        0        0     2550 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/cli/utils.py
--rw-r--r--   0        0        0     1517 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/cli/watcher.py
--rw-r--r--   0        0        0       43 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/cli/worker/__init__.py
--rw-r--r--   0        0        0     5805 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/cli/worker/args.py
--rw-r--r--   0        0        0      628 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/cli/worker/cmd.py
--rw-r--r--   0        0        0     1742 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/cli/worker/log_collector.py
--rw-r--r--   0        0        0     8307 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/cli/worker/process_manager.py
--rw-r--r--   0        0        0     6603 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/cli/worker/run.py
--rw-r--r--   0        0        0     1567 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/compat.py
--rw-r--r--   0        0        0     1251 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/context.py
--rw-r--r--   0        0        0     2930 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/decor.py
--rw-r--r--   0        0        0      511 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/events.py
--rw-r--r--   0        0        0     1010 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/exceptions.py
--rw-r--r--   0        0        0       25 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/formatters/__init__.py
--rw-r--r--   0        0        0      928 2023-07-18 20:22:04.745682 taskiq-0.8.4/taskiq/formatters/json_formatter.py
--rw-r--r--   0        0        0     1887 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/funcs.py
--rw-r--r--   0        0        0     5552 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/kicker.py
--rw-r--r--   0        0        0      507 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/message.py
--rw-r--r--   0        0        0       26 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/middlewares/__init__.py
--rw-r--r--   0        0        0     4056 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/middlewares/prometheus_middleware.py
--rw-r--r--   0        0        0     2438 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/middlewares/retry_middleware.py
--rw-r--r--   0        0        0        0 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/py.typed
--rw-r--r--   0        0        0      113 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/receiver/__init__.py
--rw-r--r--   0        0        0     2799 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/receiver/params_parser.py
--rw-r--r--   0        0        0    12601 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/receiver/receiver.py
--rw-r--r--   0        0        0      237 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/result/__init__.py
--rw-r--r--   0        0        0     2084 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/result/v1.py
--rw-r--r--   0        0        0     1923 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/result/v2.py
--rw-r--r--   0        0        0       35 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/result_backends/__init__.py
--rw-r--r--   0        0        0     1268 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/result_backends/dummy.py
--rw-r--r--   0        0        0      146 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/schedule_sources/__init__.py
--rw-r--r--   0        0        0     2554 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/schedule_sources/label_based.py
--rw-r--r--   0        0        0      264 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/scheduler/__init__.py
--rw-r--r--   0        0        0     1056 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/scheduler/merge_functions.py
--rw-r--r--   0        0        0     2404 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/scheduler/scheduler.py
--rw-r--r--   0        0        0    11916 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/serialization.py
--rw-r--r--   0        0        0     1071 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/state.py
--rw-r--r--   0        0        0     4141 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/task.py
--rw-r--r--   0        0        0      900 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/utils.py
--rw-r--r--   0        0        0      106 2023-07-18 20:22:04.749682 taskiq-0.8.4/taskiq/warnings.py
--rw-r--r--   0        0        0     3637 1970-01-01 00:00:00.000000 taskiq-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-21 00:20:14.561721 taskiq-0.8.5/LICENSE
+-rw-r--r--   0        0        0     1875 2023-07-21 00:20:14.561721 taskiq-0.8.5/README.md
+-rw-r--r--   0        0        0     3007 2023-07-21 00:20:14.565721 taskiq-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0     2022 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/__init__.py
+-rw-r--r--   0        0        0     2093 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/__main__.py
+-rw-r--r--   0        0        0      194 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/abc/__init__.py
+-rw-r--r--   0        0        0    12959 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/abc/broker.py
+-rw-r--r--   0        0        0      323 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/abc/cmd.py
+-rw-r--r--   0        0        0      629 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/abc/formatter.py
+-rw-r--r--   0        0        0     3562 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/abc/middleware.py
+-rw-r--r--   0        0        0     1376 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/abc/result_backend.py
+-rw-r--r--   0        0        0     1623 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/abc/schedule_source.py
+-rw-r--r--   0        0        0      496 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/acks.py
+-rw-r--r--   0        0        0       34 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/brokers/__init__.py
+-rw-r--r--   0        0        0     5679 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/brokers/inmemory_broker.py
+-rw-r--r--   0        0        0     2197 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/brokers/shared_broker.py
+-rw-r--r--   0        0        0     2831 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/brokers/zmq_broker.py
+-rw-r--r--   0        0        0       31 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/cli/__init__.py
+-rw-r--r--   0        0        0      197 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/cli/common_args.py
+-rw-r--r--   0        0        0       37 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/cli/scheduler/__init__.py
+-rw-r--r--   0        0        0     2346 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/cli/scheduler/args.py
+-rw-r--r--   0        0        0      651 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/cli/scheduler/cmd.py
+-rw-r--r--   0        0        0     3899 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/cli/scheduler/run.py
+-rw-r--r--   0        0        0     2550 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/cli/utils.py
+-rw-r--r--   0        0        0     1517 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/cli/watcher.py
+-rw-r--r--   0        0        0       43 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/cli/worker/__init__.py
+-rw-r--r--   0        0        0     5805 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/cli/worker/args.py
+-rw-r--r--   0        0        0      628 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/cli/worker/cmd.py
+-rw-r--r--   0        0        0     1742 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/cli/worker/log_collector.py
+-rw-r--r--   0        0        0     8307 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/cli/worker/process_manager.py
+-rw-r--r--   0        0        0     6603 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/cli/worker/run.py
+-rw-r--r--   0        0        0     1567 2023-07-21 00:20:14.565721 taskiq-0.8.5/taskiq/compat.py
+-rw-r--r--   0        0        0     1251 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/context.py
+-rw-r--r--   0        0        0     2930 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/decor.py
+-rw-r--r--   0        0        0      511 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/events.py
+-rw-r--r--   0        0        0     1010 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/exceptions.py
+-rw-r--r--   0        0        0       25 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/formatters/__init__.py
+-rw-r--r--   0        0        0      928 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/formatters/json_formatter.py
+-rw-r--r--   0        0        0     1887 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/funcs.py
+-rw-r--r--   0        0        0     5552 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/kicker.py
+-rw-r--r--   0        0        0      507 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/message.py
+-rw-r--r--   0        0        0       26 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/middlewares/__init__.py
+-rw-r--r--   0        0        0     4056 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/middlewares/prometheus_middleware.py
+-rw-r--r--   0        0        0     2438 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/middlewares/retry_middleware.py
+-rw-r--r--   0        0        0        0 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/py.typed
+-rw-r--r--   0        0        0      113 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/receiver/__init__.py
+-rw-r--r--   0        0        0     2799 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/receiver/params_parser.py
+-rw-r--r--   0        0        0    12601 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/receiver/receiver.py
+-rw-r--r--   0        0        0      237 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/result/__init__.py
+-rw-r--r--   0        0        0     2084 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/result/v1.py
+-rw-r--r--   0        0        0     1923 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/result/v2.py
+-rw-r--r--   0        0        0       35 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/result_backends/__init__.py
+-rw-r--r--   0        0        0     1268 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/result_backends/dummy.py
+-rw-r--r--   0        0        0      146 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/schedule_sources/__init__.py
+-rw-r--r--   0        0        0     2554 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/schedule_sources/label_based.py
+-rw-r--r--   0        0        0      264 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/scheduler/__init__.py
+-rw-r--r--   0        0        0     1056 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/scheduler/merge_functions.py
+-rw-r--r--   0        0        0     2404 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/scheduler/scheduler.py
+-rw-r--r--   0        0        0    11916 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/serialization.py
+-rw-r--r--   0        0        0     1071 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/state.py
+-rw-r--r--   0        0        0     4141 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/task.py
+-rw-r--r--   0        0        0      900 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/utils.py
+-rw-r--r--   0        0        0      106 2023-07-21 00:20:14.569721 taskiq-0.8.5/taskiq/warnings.py
+-rw-r--r--   0        0        0     3637 1970-01-01 00:00:00.000000 taskiq-0.8.5/PKG-INFO
```

### Comparing `taskiq-0.8.4/LICENSE` & `taskiq-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/README.md` & `taskiq-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/pyproject.toml` & `taskiq-0.8.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq"
-version = "0.8.4"
+version = "0.8.5"
 description = "Distributed task queue with full async support"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 maintainers = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 repository = "https://github.com/taskiq-python/taskiq"
 homepage = "https://taskiq-python.github.io/"
 documentation = "https://taskiq-python.github.io/"
```

### Comparing `taskiq-0.8.4/taskiq/__init__.py` & `taskiq-0.8.5/taskiq/__init__.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/__main__.py` & `taskiq-0.8.5/taskiq/__main__.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/abc/broker.py` & `taskiq-0.8.5/taskiq/abc/broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/abc/formatter.py` & `taskiq-0.8.5/taskiq/abc/formatter.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/abc/middleware.py` & `taskiq-0.8.5/taskiq/abc/middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/abc/result_backend.py` & `taskiq-0.8.5/taskiq/abc/result_backend.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/abc/schedule_source.py` & `taskiq-0.8.5/taskiq/abc/schedule_source.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/brokers/inmemory_broker.py` & `taskiq-0.8.5/taskiq/brokers/inmemory_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/brokers/shared_broker.py` & `taskiq-0.8.5/taskiq/brokers/shared_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/brokers/zmq_broker.py` & `taskiq-0.8.5/taskiq/brokers/zmq_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/cli/scheduler/args.py` & `taskiq-0.8.5/taskiq/cli/scheduler/args.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 @dataclass
 class SchedulerArgs:
     """Arguments for scheduler."""
 
     scheduler: Union[str, TaskiqScheduler]
     modules: List[str]
     log_level: str = LogLevel.INFO.name
+    configure_logging: bool = True
     fs_discover: bool = False
     tasks_pattern: str = "tasks.py"
 
     @classmethod
     def from_cli(cls, args: Optional[Sequence[str]] = None) -> "SchedulerArgs":
         """
         Build scheduler args from CLI arguments.
@@ -55,8 +56,14 @@
         )
         parser.add_argument(
             "--log-level",
             default=LogLevel.INFO.name,
             choices=[level.name for level in LogLevel],
             help="scheduler log level",
         )
+        parser.add_argument(
+            "--no-configure-logging",
+            action="store_false",
+            dest="configure_logging",
+            help="Use this parameter if your application configures custom logging.",
+        )
         return cls(**parser.parse_args(args).__dict__)
```

### Comparing `taskiq-0.8.4/taskiq/cli/scheduler/cmd.py` & `taskiq-0.8.5/taskiq/cli/scheduler/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/cli/scheduler/run.py` & `taskiq-0.8.5/taskiq/cli/scheduler/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,22 +78,24 @@
     if not isinstance(scheduler, TaskiqScheduler):
         print(  # noqa: WPS421
             "Imported scheduler is not a subclass of TaskiqScheduler.",
         )
         exit(1)  # noqa: WPS421
     scheduler.broker.is_scheduler_process = True
     import_tasks(args.modules, args.tasks_pattern, args.fs_discover)
-    basicConfig(
-        level=getLevelName(args.log_level),
-        format=(
-            "[%(asctime)s][%(levelname)-7s]"
-            "[%(module)s:%(funcName)s:%(lineno)d]"
-            " %(message)s"
-        ),
-    )
+    if args.configure_logging:
+        basicConfig(
+            level=getLevelName(args.log_level),
+            format=(
+                "[%(asctime)s][%(levelname)-7s]"
+                "[%(module)s:%(funcName)s:%(lineno)d]"
+                " %(message)s"
+            ),
+        )
+    getLogger("taskiq").setLevel(level=getLevelName(args.log_level))
     for source in scheduler.sources:
         await source.startup()
     loop = asyncio.get_event_loop()
     tasks: "List[ScheduledTask]" = []
     loop.create_task(schedules_updater(scheduler, tasks))
     logger.info("Starting scheduler.")
     await scheduler.startup()
```

### Comparing `taskiq-0.8.4/taskiq/cli/utils.py` & `taskiq-0.8.5/taskiq/cli/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/cli/watcher.py` & `taskiq-0.8.5/taskiq/cli/watcher.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/cli/worker/args.py` & `taskiq-0.8.5/taskiq/cli/worker/args.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/cli/worker/cmd.py` & `taskiq-0.8.5/taskiq/cli/worker/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/cli/worker/log_collector.py` & `taskiq-0.8.5/taskiq/cli/worker/log_collector.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/cli/worker/process_manager.py` & `taskiq-0.8.5/taskiq/cli/worker/process_manager.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/cli/worker/run.py` & `taskiq-0.8.5/taskiq/cli/worker/run.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/compat.py` & `taskiq-0.8.5/taskiq/compat.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/context.py` & `taskiq-0.8.5/taskiq/context.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/decor.py` & `taskiq-0.8.5/taskiq/decor.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/exceptions.py` & `taskiq-0.8.5/taskiq/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/formatters/json_formatter.py` & `taskiq-0.8.5/taskiq/formatters/json_formatter.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/funcs.py` & `taskiq-0.8.5/taskiq/funcs.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/kicker.py` & `taskiq-0.8.5/taskiq/kicker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/middlewares/prometheus_middleware.py` & `taskiq-0.8.5/taskiq/middlewares/prometheus_middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/middlewares/retry_middleware.py` & `taskiq-0.8.5/taskiq/middlewares/retry_middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/receiver/params_parser.py` & `taskiq-0.8.5/taskiq/receiver/params_parser.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/receiver/receiver.py` & `taskiq-0.8.5/taskiq/receiver/receiver.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/result/v1.py` & `taskiq-0.8.5/taskiq/result/v1.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/result/v2.py` & `taskiq-0.8.5/taskiq/result/v2.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/result_backends/dummy.py` & `taskiq-0.8.5/taskiq/result_backends/dummy.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/schedule_sources/label_based.py` & `taskiq-0.8.5/taskiq/schedule_sources/label_based.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/scheduler/merge_functions.py` & `taskiq-0.8.5/taskiq/scheduler/merge_functions.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/scheduler/scheduler.py` & `taskiq-0.8.5/taskiq/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/serialization.py` & `taskiq-0.8.5/taskiq/serialization.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/state.py` & `taskiq-0.8.5/taskiq/state.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/task.py` & `taskiq-0.8.5/taskiq/task.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/taskiq/utils.py` & `taskiq-0.8.5/taskiq/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.4/PKG-INFO` & `taskiq-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq
-Version: 0.8.4
+Version: 0.8.5
 Summary: Distributed task queue with full async support
 Home-page: https://taskiq-python.github.io/
 License: LICENSE
 Keywords: taskiq,tasks,distributed,async
 Author: Pavel Kirilin
 Author-email: win10@list.ru
 Maintainer: Pavel Kirilin
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: taskiq Version: 0.8.4 Summary: Distributed task
+Metadata-Version: 2.1 Name: taskiq Version: 0.8.5 Summary: Distributed task
 queue with full async support Home-page: https://taskiq-python.github.io/
 License: LICENSE Keywords: taskiq,tasks,distributed,async Author: Pavel Kirilin
 Author-email: win10@list.ru Maintainer: Pavel Kirilin Maintainer-email:
 win10@list.ru Requires-Python: >=3.8.1,<4.0.0 Classifier: Development Status ::
 3 - Alpha Classifier: Intended Audience :: Developers Classifier: License ::
 Other/Proprietary License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

