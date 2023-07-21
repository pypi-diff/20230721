# Comparing `tmp/troncos-4.0.1.tar.gz` & `tmp/troncos-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troncos-4.0.1.tar", max compression
+gzip compressed data, was "troncos-4.0.2.tar", max compression
```

## Comparing `troncos-4.0.1.tar` & `troncos-4.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1077 2023-07-13 09:38:03.586661 troncos-4.0.1/LICENSE
--rw-r--r--   0        0        0     8203 2023-07-13 09:38:03.586661 troncos-4.0.1/README.md
--rw-r--r--   0        0        0     2459 2023-07-13 09:38:03.586661 troncos-4.0.1/pyproject.toml
--rw-r--r--   0        0        0      291 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/asgi/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/asgi/logging/__init__.py
--rw-r--r--   0        0        0     5297 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/asgi/logging/middleware.py
--rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/asgi/profiling/__init__.py
--rw-r--r--   0        0        0      576 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/asgi/profiling/app.py
--rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/celery/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/celery/logging/__init__.py
--rw-r--r--   0        0        0      969 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/celery/logging/signals.py
--rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/django/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/django/logging/__init__.py
--rw-r--r--   0        0        0     2354 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/django/logging/middleware.py
--rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/django/profiling/__init__.py
--rw-r--r--   0        0        0      259 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/django/profiling/views.py
--rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/logging/__init__.py
--rw-r--r--   0        0        0     3455 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/logging/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/starlette/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/starlette/profiling/__init__.py
--rw-r--r--   0        0        0      291 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/starlette/profiling/views.py
--rw-r--r--   0        0        0     4300 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/structlog/__init__.py
--rw-r--r--   0        0        0      906 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/structlog/processors.py
--rw-r--r--   0        0        0       82 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/profiling/__init__.py
--rw-r--r--   0        0        0      192 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/profiling/auto.py
--rw-r--r--   0        0        0        0 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/profiling/bootstrap/__init__.py
--rw-r--r--   0        0        0      439 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/profiling/bootstrap/profile.py
--rw-r--r--   0        0        0      343 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/profiling/bootstrap/start.py
--rw-r--r--   0        0        0     1814 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/profiling/profiler.py
--rw-r--r--   0        0        0     1155 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/profiling/pyroscope.py
--rw-r--r--   0        0        0        0 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/py.typed
--rw-r--r--   0        0        0      690 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/tracing/__init__.py
--rw-r--r--   0        0        0       82 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/tracing/_enums.py
--rw-r--r--   0        0        0     2053 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/tracing/_otel.py
--rw-r--r--   0        0        0     4582 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/tracing/_span.py
--rw-r--r--   0        0        0     2675 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/tracing/_writer.py
--rw-r--r--   0        0        0     7585 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/tracing/decorators.py
--rw-r--r--   0        0        0     9237 1970-01-01 00:00:00.000000 troncos-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-21 10:51:58.299003 troncos-4.0.2/LICENSE
+-rw-r--r--   0        0        0     8203 2023-07-21 10:51:58.299003 troncos-4.0.2/README.md
+-rw-r--r--   0        0        0     2518 2023-07-21 10:51:58.299003 troncos-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0      291 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/contrib/asgi/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/contrib/asgi/logging/__init__.py
+-rw-r--r--   0        0        0     5297 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/contrib/asgi/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/contrib/asgi/profiling/__init__.py
+-rw-r--r--   0        0        0      576 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/contrib/asgi/profiling/app.py
+-rw-r--r--   0        0        0        0 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/contrib/celery/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/contrib/celery/logging/__init__.py
+-rw-r--r--   0        0        0      969 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/contrib/celery/logging/signals.py
+-rw-r--r--   0        0        0        0 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/contrib/django/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/django/logging/__init__.py
+-rw-r--r--   0        0        0     2354 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/django/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/django/profiling/__init__.py
+-rw-r--r--   0        0        0      259 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/django/profiling/views.py
+-rw-r--r--   0        0        0        0 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/logging/__init__.py
+-rw-r--r--   0        0        0     3455 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/logging/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/starlette/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/starlette/profiling/__init__.py
+-rw-r--r--   0        0        0      291 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/starlette/profiling/views.py
+-rw-r--r--   0        0        0     5176 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/structlog/__init__.py
+-rw-r--r--   0        0        0      906 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/structlog/processors.py
+-rw-r--r--   0        0        0       82 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/profiling/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/profiling/auto.py
+-rw-r--r--   0        0        0        0 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/profiling/bootstrap/__init__.py
+-rw-r--r--   0        0        0      439 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/profiling/bootstrap/profile.py
+-rw-r--r--   0        0        0      343 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/profiling/bootstrap/start.py
+-rw-r--r--   0        0        0     1814 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/profiling/profiler.py
+-rw-r--r--   0        0        0     1155 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/profiling/pyroscope.py
+-rw-r--r--   0        0        0        0 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/py.typed
+-rw-r--r--   0        0        0      690 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/tracing/__init__.py
+-rw-r--r--   0        0        0       82 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/tracing/_enums.py
+-rw-r--r--   0        0        0     2053 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/tracing/_otel.py
+-rw-r--r--   0        0        0     4582 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/tracing/_span.py
+-rw-r--r--   0        0        0     2675 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/tracing/_writer.py
+-rw-r--r--   0        0        0     7585 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/tracing/decorators.py
+-rw-r--r--   0        0        0     9329 1970-01-01 00:00:00.000000 troncos-4.0.2/PKG-INFO
```

### Comparing `troncos-4.0.1/LICENSE` & `troncos-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `troncos-4.0.1/README.md` & `troncos-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `troncos-4.0.1/pyproject.toml` & `troncos-4.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troncos"
-version = "4.0.1"
+version = "4.0.2"
 description = "Collection of Python logging, tracing and profiling tools"
 authors = [
     "Guðmundur Björn Birkisson <gudmundur.birkisson@oda.com>",
     "Karl Fredrik Haugland <karlfredrik.haugland@oda.com>",
     "Eirik Martiniussen Sylliaas <eirik.sylliaas@oda.com>",
 ]
 license = "MIT"
@@ -16,19 +16,21 @@
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 ddtrace = "1.15.0"
 opentelemetry-sdk = "1.18.0"
 opentelemetry-exporter-otlp-proto-http = "1.18.0"
 opentelemetry-exporter-otlp-proto-grpc = {version = "1.18.0", optional = true}
+structlog-sentry = {version = "^2.0.3", optional = true}
 python-ipware = "^0.9.0"
 pyroscope-io = "^0.8.3"
 
 [tool.poetry.extras]
 grpc = ["opentelemetry-exporter-otlp-proto-grpc"]
+sentry = ["structlog-sentry"]
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.1"
 pytest = "^7.2.1"
@@ -41,15 +43,14 @@
 django-environ = "^0.9.0"
 pytest-benchmark = "^4.0.0"
 snakeviz = "^2.2.0"
 django = "^4.2.1"
 starlette = "^0.27.0"
 structlog = "^23.1.0"
 celery = "^5.2.7"
-structlog-sentry = "^2.0.3"
 ipython = "^8.14.0"
 
 
 [tool.black]
 target-version = ['py311']
 line-length = 88
 include = '\.pyi?$'
```

### Comparing `troncos-4.0.1/troncos/contrib/asgi/logging/middleware.py` & `troncos-4.0.2/troncos/contrib/asgi/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.1/troncos/contrib/asgi/profiling/app.py` & `troncos-4.0.2/troncos/contrib/asgi/profiling/app.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.1/troncos/contrib/celery/logging/signals.py` & `troncos-4.0.2/troncos/contrib/celery/logging/signals.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.1/troncos/contrib/django/logging/middleware.py` & `troncos-4.0.2/troncos/contrib/django/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.1/troncos/contrib/logging/tools/__init__.py` & `troncos-4.0.2/troncos/contrib/logging/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.1/troncos/contrib/structlog/__init__.py` & `troncos-4.0.2/troncos/contrib/structlog/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import logging.config
+from typing import Any, Iterable, Optional
 
 import structlog
 
 from troncos.contrib.structlog.processors import (
     LogfmtRenderer,
     trace_injection_processor,
 )
@@ -34,26 +35,47 @@
     shared_processors.insert(
         format_exc_info_index,
         SentryProcessor(level=logging.INFO, event_level=logging.ERROR),
     )
 
 
 def configure_structlog(
-    *, configure_logging: bool = True, format: str = "text", level: str = "INFO"
+    *,
+    configure_logging: bool = True,
+    format: str = "text",
+    level: str = "INFO",
+    extra_processors: Optional[Iterable[structlog.typing.Processor]] = None,
+    extra_loggers: Optional[dict[str, dict[str, Any]]] = None,
 ) -> None:
     """
     Helper method to configure Structlog.
 
     Using this is not required, you can configure Structlog
     manually in your application.
 
     configure_logging=True lets you use structlog to render logs from
     logging.getLogger, this is used to get an unified log output.
+
+    If `extra_processors` is set, these will be inserted to the list of processors
+    just before `format_exc_info`.
+
+    If `extra_loggers` is set, it will be unpacked into the `loggers` directive of
+    the dictconfig dict. The `handler` value for these loggers must be `"default"`
     """
 
+    extra_loggers = extra_loggers or {}
+    extra_processors = extra_processors or []
+
+    if extra_processors:
+        _format_exc_info_index = shared_processors.index(
+            structlog.processors.format_exc_info
+        )
+        for index, proc in enumerate(extra_processors):
+            shared_processors.insert(_format_exc_info_index + index, proc)
+
     processor: structlog.types.Processor
 
     if format == "text":
         processor = structlog.dev.ConsoleRenderer(colors=True)
     elif format == "json":
         processor = structlog.processors.JSONRenderer()
     elif format == "logfmt":
@@ -81,14 +103,15 @@
             },
             "loggers": {
                 "": {
                     "handlers": ["default"],
                     "level": level,
                     "propagate": True,
                 },
+                **extra_loggers,
             },
         }
 
         logging.config.dictConfig(config)
 
     structlog_processors: list[structlog.types.Processor] = [
         # Merge contextvars into the event dict.
```

### Comparing `troncos-4.0.1/troncos/contrib/structlog/processors.py` & `troncos-4.0.2/troncos/contrib/structlog/processors.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.1/troncos/profiling/profiler.py` & `troncos-4.0.2/troncos/profiling/profiler.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.1/troncos/profiling/pyroscope.py` & `troncos-4.0.2/troncos/profiling/pyroscope.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.1/troncos/tracing/__init__.py` & `troncos-4.0.2/troncos/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.1/troncos/tracing/_otel.py` & `troncos-4.0.2/troncos/tracing/_otel.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.1/troncos/tracing/_span.py` & `troncos-4.0.2/troncos/tracing/_span.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.1/troncos/tracing/_writer.py` & `troncos-4.0.2/troncos/tracing/_writer.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.1/troncos/tracing/decorators.py` & `troncos-4.0.2/troncos/tracing/decorators.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.1/PKG-INFO` & `troncos-4.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: troncos
-Version: 4.0.1
+Version: 4.0.2
 Summary: Collection of Python logging, tracing and profiling tools
 Home-page: https://github.com/kolonialno/troncos
 License: MIT
 Keywords: logs,traces,opentelemetry
 Author: Guðmundur Björn Birkisson
 Author-email: gudmundur.birkisson@oda.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: grpc
+Provides-Extra: sentry
 Requires-Dist: ddtrace (==1.15.0)
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc (==1.18.0) ; extra == "grpc"
 Requires-Dist: opentelemetry-exporter-otlp-proto-http (==1.18.0)
 Requires-Dist: opentelemetry-sdk (==1.18.0)
 Requires-Dist: pyroscope-io (>=0.8.3,<0.9.0)
 Requires-Dist: python-ipware (>=0.9.0,<0.10.0)
+Requires-Dist: structlog-sentry (>=2.0.3,<3.0.0) ; extra == "sentry"
 Project-URL: Documentation, https://github.com/kolonialno/troncos
 Project-URL: Repository, https://github.com/kolonialno/troncos
 Description-Content-Type: text/markdown
 
 <h1 align="center" style="border-bottom: 0">
   🪵<br>
   Troncos <br/>
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: troncos Version: 4.0.1 Summary: Collection of
+Metadata-Version: 2.1 Name: troncos Version: 4.0.2 Summary: Collection of
 Python logging, tracing and profiling tools Home-page: https://github.com/
 kolonialno/troncos License: MIT Keywords: logs,traces,opentelemetry Author:
 GuÃ°mundur BjÃ¶rn Birkisson Author-email: gudmundur.birkisson@oda.com Requires-
 Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: grpc Requires-Dist: ddtrace (==1.15.0) Requires-Dist:
-opentelemetry-exporter-otlp-proto-grpc (==1.18.0) ; extra == "grpc" Requires-
-Dist: opentelemetry-exporter-otlp-proto-http (==1.18.0) Requires-Dist:
-opentelemetry-sdk (==1.18.0) Requires-Dist: pyroscope-io (>=0.8.3,<0.9.0)
-Requires-Dist: python-ipware (>=0.9.0,<0.10.0) Project-URL: Documentation,
-https://github.com/kolonialno/troncos Project-URL: Repository, https://
-github.com/kolonialno/troncos Description-Content-Type: text/markdown
+Provides-Extra: grpc Provides-Extra: sentry Requires-Dist: ddtrace (==1.15.0)
+Requires-Dist: opentelemetry-exporter-otlp-proto-grpc (==1.18.0) ; extra ==
+"grpc" Requires-Dist: opentelemetry-exporter-otlp-proto-http (==1.18.0)
+Requires-Dist: opentelemetry-sdk (==1.18.0) Requires-Dist: pyroscope-io
+(>=0.8.3,<0.9.0) Requires-Dist: python-ipware (>=0.9.0,<0.10.0) Requires-Dist:
+structlog-sentry (>=2.0.3,<3.0.0) ; extra == "sentry" Project-URL:
+Documentation, https://github.com/kolonialno/troncos Project-URL: Repository,
+https://github.com/kolonialno/troncos Description-Content-Type: text/markdown
                                   ****** ðªµ
                                    Troncos
                                      ******
           Collection of Python logging, tracing and profiling tools
        [CI_status] [https://img.shields.io/pypi/v/troncos.svg] [https://
 img.shields.io/pypi/pyversions/troncos] [https://img.shields.io/github/license/
                             kolonialno/troncos.svg]
```

