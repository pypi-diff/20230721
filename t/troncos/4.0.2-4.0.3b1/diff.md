# Comparing `tmp/troncos-4.0.2.tar.gz` & `tmp/troncos-4.0.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troncos-4.0.2.tar", max compression
+gzip compressed data, was "troncos-4.0.3b1.tar", max compression
```

## Comparing `troncos-4.0.2.tar` & `troncos-4.0.3b1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1077 2023-07-21 10:51:58.299003 troncos-4.0.2/LICENSE
--rw-r--r--   0        0        0     8203 2023-07-21 10:51:58.299003 troncos-4.0.2/README.md
--rw-r--r--   0        0        0     2518 2023-07-21 10:51:58.299003 troncos-4.0.2/pyproject.toml
--rw-r--r--   0        0        0      291 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/contrib/asgi/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/contrib/asgi/logging/__init__.py
--rw-r--r--   0        0        0     5297 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/contrib/asgi/logging/middleware.py
--rw-r--r--   0        0        0        0 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/contrib/asgi/profiling/__init__.py
--rw-r--r--   0        0        0      576 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/contrib/asgi/profiling/app.py
--rw-r--r--   0        0        0        0 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/contrib/celery/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/contrib/celery/logging/__init__.py
--rw-r--r--   0        0        0      969 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/contrib/celery/logging/signals.py
--rw-r--r--   0        0        0        0 2023-07-21 10:51:58.299003 troncos-4.0.2/troncos/contrib/django/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/django/logging/__init__.py
--rw-r--r--   0        0        0     2354 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/django/logging/middleware.py
--rw-r--r--   0        0        0        0 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/django/profiling/__init__.py
--rw-r--r--   0        0        0      259 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/django/profiling/views.py
--rw-r--r--   0        0        0        0 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/logging/__init__.py
--rw-r--r--   0        0        0     3455 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/logging/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/starlette/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/starlette/profiling/__init__.py
--rw-r--r--   0        0        0      291 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/starlette/profiling/views.py
--rw-r--r--   0        0        0     5176 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/structlog/__init__.py
--rw-r--r--   0        0        0      906 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/contrib/structlog/processors.py
--rw-r--r--   0        0        0       82 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/profiling/__init__.py
--rw-r--r--   0        0        0      192 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/profiling/auto.py
--rw-r--r--   0        0        0        0 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/profiling/bootstrap/__init__.py
--rw-r--r--   0        0        0      439 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/profiling/bootstrap/profile.py
--rw-r--r--   0        0        0      343 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/profiling/bootstrap/start.py
--rw-r--r--   0        0        0     1814 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/profiling/profiler.py
--rw-r--r--   0        0        0     1155 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/profiling/pyroscope.py
--rw-r--r--   0        0        0        0 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/py.typed
--rw-r--r--   0        0        0      690 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/tracing/__init__.py
--rw-r--r--   0        0        0       82 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/tracing/_enums.py
--rw-r--r--   0        0        0     2053 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/tracing/_otel.py
--rw-r--r--   0        0        0     4582 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/tracing/_span.py
--rw-r--r--   0        0        0     2675 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/tracing/_writer.py
--rw-r--r--   0        0        0     7585 2023-07-21 10:51:58.303002 troncos-4.0.2/troncos/tracing/decorators.py
--rw-r--r--   0        0        0     9329 1970-01-01 00:00:00.000000 troncos-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-21 12:51:31.625196 troncos-4.0.3b1/LICENSE
+-rw-r--r--   0        0        0     8203 2023-07-21 12:51:31.625196 troncos-4.0.3b1/README.md
+-rw-r--r--   0        0        0     2520 2023-07-21 12:51:31.625196 troncos-4.0.3b1/pyproject.toml
+-rw-r--r--   0        0        0      291 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/asgi/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/asgi/logging/__init__.py
+-rw-r--r--   0        0        0     5297 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/asgi/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/asgi/profiling/__init__.py
+-rw-r--r--   0        0        0      576 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/asgi/profiling/app.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/celery/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/celery/logging/__init__.py
+-rw-r--r--   0        0        0      969 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/celery/logging/signals.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/django/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/django/logging/__init__.py
+-rw-r--r--   0        0        0     2361 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/django/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/django/profiling/__init__.py
+-rw-r--r--   0        0        0      259 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/django/profiling/views.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/logging/__init__.py
+-rw-r--r--   0        0        0     3455 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/logging/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/starlette/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/starlette/profiling/__init__.py
+-rw-r--r--   0        0        0      291 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/starlette/profiling/views.py
+-rw-r--r--   0        0        0     5176 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/contrib/structlog/__init__.py
+-rw-r--r--   0        0        0      906 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/contrib/structlog/processors.py
+-rw-r--r--   0        0        0       82 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/profiling/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/profiling/auto.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/profiling/bootstrap/__init__.py
+-rw-r--r--   0        0        0      439 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/profiling/bootstrap/profile.py
+-rw-r--r--   0        0        0      343 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/profiling/bootstrap/start.py
+-rw-r--r--   0        0        0     1814 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/profiling/profiler.py
+-rw-r--r--   0        0        0     1155 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/profiling/pyroscope.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/py.typed
+-rw-r--r--   0        0        0      690 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/tracing/__init__.py
+-rw-r--r--   0        0        0       82 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/tracing/_enums.py
+-rw-r--r--   0        0        0     2053 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/tracing/_otel.py
+-rw-r--r--   0        0        0     4582 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/tracing/_span.py
+-rw-r--r--   0        0        0     2675 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/tracing/_writer.py
+-rw-r--r--   0        0        0     7585 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/tracing/decorators.py
+-rw-r--r--   0        0        0     9331 1970-01-01 00:00:00.000000 troncos-4.0.3b1/PKG-INFO
```

### Comparing `troncos-4.0.2/LICENSE` & `troncos-4.0.3b1/LICENSE`

 * *Files identical despite different names*

### Comparing `troncos-4.0.2/README.md` & `troncos-4.0.3b1/README.md`

 * *Files identical despite different names*

### Comparing `troncos-4.0.2/pyproject.toml` & `troncos-4.0.3b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troncos"
-version = "4.0.2"
+version = "4.0.3b1"
 description = "Collection of Python logging, tracing and profiling tools"
 authors = [
     "Guðmundur Björn Birkisson <gudmundur.birkisson@oda.com>",
     "Karl Fredrik Haugland <karlfredrik.haugland@oda.com>",
     "Eirik Martiniussen Sylliaas <eirik.sylliaas@oda.com>",
 ]
 license = "MIT"
```

### Comparing `troncos-4.0.2/troncos/contrib/asgi/logging/middleware.py` & `troncos-4.0.3b1/troncos/contrib/asgi/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.2/troncos/contrib/asgi/profiling/app.py` & `troncos-4.0.3b1/troncos/contrib/asgi/profiling/app.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.2/troncos/contrib/celery/logging/signals.py` & `troncos-4.0.3b1/troncos/contrib/celery/logging/signals.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.2/troncos/contrib/django/logging/middleware.py` & `troncos-4.0.3b1/troncos/contrib/django/logging/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
 from typing import Any
 
 from asgiref.sync import iscoroutinefunction
 from django.http import HttpRequest, HttpResponse
 from django.utils.decorators import sync_and_async_middleware
-from ipware import IpWare
+from ipware.ipware import IpWare
 
 try:
     from structlog import get_logger
 except ImportError:
     raise RuntimeError(
         "Structlog must be installed to use the asgi logging middleware."
     )
```

### Comparing `troncos-4.0.2/troncos/contrib/logging/tools/__init__.py` & `troncos-4.0.3b1/troncos/contrib/logging/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.2/troncos/contrib/structlog/__init__.py` & `troncos-4.0.3b1/troncos/contrib/structlog/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.2/troncos/contrib/structlog/processors.py` & `troncos-4.0.3b1/troncos/contrib/structlog/processors.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.2/troncos/profiling/profiler.py` & `troncos-4.0.3b1/troncos/profiling/profiler.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.2/troncos/profiling/pyroscope.py` & `troncos-4.0.3b1/troncos/profiling/pyroscope.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.2/troncos/tracing/__init__.py` & `troncos-4.0.3b1/troncos/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.2/troncos/tracing/_otel.py` & `troncos-4.0.3b1/troncos/tracing/_otel.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.2/troncos/tracing/_span.py` & `troncos-4.0.3b1/troncos/tracing/_span.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.2/troncos/tracing/_writer.py` & `troncos-4.0.3b1/troncos/tracing/_writer.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.2/troncos/tracing/decorators.py` & `troncos-4.0.3b1/troncos/tracing/decorators.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.2/PKG-INFO` & `troncos-4.0.3b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troncos
-Version: 4.0.2
+Version: 4.0.3b1
 Summary: Collection of Python logging, tracing and profiling tools
 Home-page: https://github.com/kolonialno/troncos
 License: MIT
 Keywords: logs,traces,opentelemetry
 Author: Guðmundur Björn Birkisson
 Author-email: gudmundur.birkisson@oda.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: troncos Version: 4.0.2 Summary: Collection of
+Metadata-Version: 2.1 Name: troncos Version: 4.0.3b1 Summary: Collection of
 Python logging, tracing and profiling tools Home-page: https://github.com/
 kolonialno/troncos License: MIT Keywords: logs,traces,opentelemetry Author:
 GuÃ°mundur BjÃ¶rn Birkisson Author-email: gudmundur.birkisson@oda.com Requires-
 Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: grpc Provides-Extra: sentry Requires-Dist: ddtrace (==1.15.0)
```

