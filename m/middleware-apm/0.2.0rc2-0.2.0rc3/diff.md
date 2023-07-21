# Comparing `tmp/middleware-apm-0.2.0rc2.tar.gz` & `tmp/middleware-apm-0.2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "middleware-apm-0.2.0rc2.tar", last modified: Tue Jul 18 11:10:40 2023, max compression
+gzip compressed data, was "middleware-apm-0.2.0rc3.tar", last modified: Fri Jul 21 05:59:53 2023, max compression
```

## Comparing `middleware-apm-0.2.0rc2.tar` & `middleware-apm-0.2.0rc3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:10:40.608655 middleware-apm-0.2.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 11:10:17.000000 middleware-apm-0.2.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-18 11:10:40.608655 middleware-apm-0.2.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 11:10:17.000000 middleware-apm-0.2.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:10:40.608655 middleware-apm-0.2.0rc2/middleware_apm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-18 11:10:40.000000 middleware-apm-0.2.0rc2/middleware_apm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-18 11:10:40.000000 middleware-apm-0.2.0rc2/middleware_apm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 11:10:40.000000 middleware-apm-0.2.0rc2/middleware_apm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-18 11:10:40.000000 middleware-apm-0.2.0rc2/middleware_apm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-18 11:10:40.000000 middleware-apm-0.2.0rc2/middleware_apm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 11:10:40.000000 middleware-apm-0.2.0rc2/middleware_apm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 11:10:40.608655 middleware-apm-0.2.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-18 11:10:17.000000 middleware-apm-0.2.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:10:40.608655 middleware-apm-0.2.0rc2/source/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-18 11:10:17.000000 middleware-apm-0.2.0rc2/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-18 11:10:17.000000 middleware-apm-0.2.0rc2/source/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-18 11:10:17.000000 middleware-apm-0.2.0rc2/source/_meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-18 11:10:17.000000 middleware-apm-0.2.0rc2/source/_tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-18 11:10:17.000000 middleware-apm-0.2.0rc2/source/mw_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:59:53.287302 middleware-apm-0.2.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 05:59:29.000000 middleware-apm-0.2.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-21 05:59:53.287302 middleware-apm-0.2.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-21 05:59:29.000000 middleware-apm-0.2.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:59:53.283301 middleware-apm-0.2.0rc3/middleware_apm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-21 05:59:53.000000 middleware-apm-0.2.0rc3/middleware_apm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-21 05:59:53.000000 middleware-apm-0.2.0rc3/middleware_apm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 05:59:53.000000 middleware-apm-0.2.0rc3/middleware_apm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-21 05:59:53.000000 middleware-apm-0.2.0rc3/middleware_apm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-21 05:59:53.000000 middleware-apm-0.2.0rc3/middleware_apm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 05:59:53.000000 middleware-apm-0.2.0rc3/middleware_apm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:59:53.287302 middleware-apm-0.2.0rc3/mw_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-21 05:59:29.000000 middleware-apm-0.2.0rc3/mw_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-21 05:59:29.000000 middleware-apm-0.2.0rc3/mw_tracker/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-07-21 05:59:29.000000 middleware-apm-0.2.0rc3/mw_tracker/_meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-21 05:59:29.000000 middleware-apm-0.2.0rc3/mw_tracker/_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-21 05:59:29.000000 middleware-apm-0.2.0rc3/mw_tracker/_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-21 05:59:29.000000 middleware-apm-0.2.0rc3/mw_tracker/mw_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 05:59:53.287302 middleware-apm-0.2.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-21 05:59:29.000000 middleware-apm-0.2.0rc3/setup.py
```

### Comparing `middleware-apm-0.2.0rc2/LICENSE` & `middleware-apm-0.2.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `middleware-apm-0.2.0rc2/setup.py` & `middleware-apm-0.2.0rc3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 except IOError:
     requirements = []
 
 
 setuptools.setup(
 
     name="middleware-apm",
-    version="0.2.0rc2",
+    version="0.2.0rc3",
     install_requires=requirements,
     author="middleware-dev",
     description="This package is use to check the RAM and CPU Usage of Current Device.",
     long_description=open('README.md').read(),
     long_description_content_type='text/plain',
-    packages=["source"],
+    packages=["mw_tracker"],
     url = "https://github.com/middleware-labs/agent-apm-python.git",
     entry_points={
         'console_scripts': [
             'middleware-instrument = opentelemetry.instrumentation.auto_instrumentation:run',
             'middleware-bootstrap = opentelemetry.instrumentation.bootstrap:run',
         ],
     },
```

### Comparing `middleware-apm-0.2.0rc2/source/_logger.py` & `middleware-apm-0.2.0rc3/mw_tracker/_logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import logging
 
 from opentelemetry._logs import set_logger_provider
 from opentelemetry.exporter.otlp.proto.grpc._log_exporter import (
     OTLPLogExporter,
 )
-from opentelemetry.sdk._logs import LoggerProvider, LoggingHandler, LogData, LogRecord, Logger
+from opentelemetry.sdk._logs import LoggerProvider, LoggingHandler
 from opentelemetry.sdk._logs.export import BatchLogRecordProcessor
 from opentelemetry.sdk.resources import Resource
 
 mw_agent_target = os.environ.get('MW_AGENT_SERVICE', '127.0.0.1')
 
 
 def log_handler(project_name, service_name):
```

### Comparing `middleware-apm-0.2.0rc2/source/_meter.py` & `middleware-apm-0.2.0rc3/mw_tracker/_meter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 import psutil
 import os
 import threading
 import gc
 from sys import getswitchinterval
 
 from opentelemetry import metrics
-from opentelemetry.sdk.resources import Resource
 from opentelemetry.metrics import CallbackOptions, Observation
-from opentelemetry.sdk.metrics import MeterProvider
-from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
-from opentelemetry.exporter.otlp.proto.grpc.metric_exporter import OTLPMetricExporter
-
+# from opentelemetry.sdk.resources import Resource
+# from opentelemetry.sdk.metrics import MeterProvider
+# from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
+# from opentelemetry.exporter.otlp.proto.grpc.metric_exporter import OTLPMetricExporter
 
 mw_agent_target = os.environ.get('MW_AGENT_SERVICE', '127.0.0.1')
 
 
-def collect_metrics(project_name, service_name) -> None:
-    print("MeterProvider called here...")
-    metrics.set_meter_provider(
-        MeterProvider(
-            resource=Resource.create({
-                "service.name": service_name,
-                "project.name": project_name,
-                "mw.app.lang": "python",
-                "runtime.metrics.python": "true"
-            }),
-            metric_readers=[
-                PeriodicExportingMetricReader(
-                    OTLPMetricExporter(insecure=True, endpoint=mw_agent_target + ":9319")
-                )
-            ],
-        )
-    )
-    meter = metrics.get_meter("middleware-apm", "0.1.41")
+def collect_metrics() -> None:
+    # metrics.set_meter_provider(MeterProvider(
+    #     resource=Resource.create({
+    #         "service.name": service_name,
+    #         "project.name": project_name,
+    #         "mw.app.lang": "python",
+    #         "runtime.metrics.python": "true"
+    #     }),
+    #     metric_readers=[
+    #         PeriodicExportingMetricReader(
+    #             OTLPMetricExporter(insecure=True, endpoint=mw_agent_target + ":9319")
+    #         )
+    #     ],
+    # ))
+    provider = metrics.get_meter_provider()
+    meter = provider.get_meter("middleware-apm", "0.2.0")
     _generate_metrics(meter)
 
 
 def _generate_metrics(meter):
     meter.create_observable_gauge(
         "process.cpu_usage.percentage",
         unit="Percent",
@@ -138,21 +135,22 @@
         unit="Bytes",
         callbacks=[_disk_usage_total_cb, _disk_usage_used_cb, _disk_usage_free_cb],
         description="The will show the disk usage of the process"
     )
 
 
 def _cpu_usage_cb(options: CallbackOptions):
-    print("------ Metrics generated -----")
+    print("--- Metrics Generated ---")
     yield Observation(value=psutil.Process(os.getpid()).cpu_percent())
 
 
 def _ram_usage_cb(options: CallbackOptions):
     yield Observation(value=psutil.Process(os.getpid()).memory_percent())
 
+
 def _cpu_time_callback(options: CallbackOptions):
     cpu_times = psutil.Process(os.getpid()).cpu_times()
     yield Observation(value=cpu_times.user, attributes={"state": "user"})
     yield Observation(value=cpu_times.system, attributes={"state": "system"})
     yield Observation(value=cpu_times.children_user, attributes={"state": "children_user"})
     yield Observation(value=cpu_times.children_system, attributes={"state": "children_system"})
     yield Observation(value=cpu_times.iowait, attributes={"state": "iowait"})
```

### Comparing `middleware-apm-0.2.0rc2/source/_tracer.py` & `middleware-apm-0.2.0rc3/mw_tracker/_profiler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import os
 import requests, json
 import pyroscope
-from opentelemetry import trace
 
 mw_agent_target = os.environ.get('MW_AGENT_SERVICE', '127.0.0.1')
 
 
-def track(project_name, service_name, access_token="",
-          enabled_profiling=True) -> None:
-    # Profiling application, if enabled
-    if enabled_profiling and access_token != "":
+def collect_profiling(service_name, access_token="") -> None:
+    if access_token != "":
 
         # Setting Middleware Account Authentication URL
         auth_url = os.getenv('MW_AUTH_URL', 'https://app.middleware.io/api/v1/auth')
 
         # Setting Middleware Profiling Server URL
         profiling_server_url = os.getenv('MW_PROFILING_SERVER_URL', 'https://profiling.middleware.io')
 
@@ -42,32 +39,7 @@
                     print("Request failed: " + data["error"])
             else:
                 print("Request failed with status code: " + str(response.status_code))
         except Exception as e:
             print("Error making request:", e)
     else:
         print("Profiling is not enabled or access token is empty")
-
-    # Setting values for tracing application
-    if type(project_name) is not str:
-        print("project name must be a string")
-        return
-    if type(service_name) is not str:
-        print("service name must be a string")
-        return
-
-
-def record_error(error):
-    span = trace.get_current_span()
-    span.record_exception(error)
-    span.set_status(trace.Status(trace.StatusCode.ERROR, str(error)))
-
-
-# def set_attribute(name, value):
-#     if type(name) is not str:
-#         print("name must be a string")
-#         return
-#     if type(value) is not str:
-#         print("value must be a string")
-#         return
-#     span = trace.get_current_span()
-#     span.set_attribute(name, value)
```

