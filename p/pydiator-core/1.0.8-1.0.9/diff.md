# Comparing `tmp/pydiator-core-1.0.8.tar.gz` & `tmp/pydiator-core-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiator-core-1.0.8.tar", last modified: Mon Jan 11 19:35:17 2021, max compression
+gzip compressed data, was "pydiator-core-1.0.9.tar", last modified: Tue Jan 12 19:52:35 2021, max compression
```

## Comparing `pydiator-core-1.0.8.tar` & `pydiator-core-1.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-11 19:35:17.169312 pydiator-core-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)     8043 2021-01-11 19:35:17.169312 pydiator-core-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6150 2021-01-11 19:35:06.000000 pydiator-core-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-11 19:35:17.165312 pydiator-core-1.0.8/pydiator_core/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-11 19:35:06.000000 pydiator-core-1.0.8/pydiator_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      791 2021-01-11 19:35:06.000000 pydiator-core-1.0.8/pydiator_core/default_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (116)     3010 2021-01-11 19:35:06.000000 pydiator-core-1.0.8/pydiator_core/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (116)      626 2021-01-11 19:35:06.000000 pydiator-core-1.0.8/pydiator_core/logger.py
--rw-r--r--   0 runner    (1001) docker     (116)     2148 2021-01-11 19:35:06.000000 pydiator-core-1.0.8/pydiator_core/mediatr.py
--rw-r--r--   0 runner    (1001) docker     (116)     2046 2021-01-11 19:35:06.000000 pydiator-core-1.0.8/pydiator_core/mediatr_container.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-11 19:35:17.165312 pydiator-core-1.0.8/pydiator_core/pipelines/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-11 19:35:06.000000 pydiator-core-1.0.8/pydiator_core/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2288 2021-01-11 19:35:06.000000 pydiator-core-1.0.8/pydiator_core/pipelines/cache_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (116)     1268 2021-01-11 19:35:06.000000 pydiator-core-1.0.8/pydiator_core/pipelines/log_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (116)     1852 2021-01-11 19:35:06.000000 pydiator-core-1.0.8/pydiator_core/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-11 19:35:17.165312 pydiator-core-1.0.8/pydiator_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     8043 2021-01-11 19:35:16.000000 pydiator-core-1.0.8/pydiator_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      670 2021-01-11 19:35:17.000000 pydiator-core-1.0.8/pydiator_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-11 19:35:16.000000 pydiator-core-1.0.8/pydiator_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       20 2021-01-11 19:35:16.000000 pydiator-core-1.0.8/pydiator_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-11 19:35:17.169312 pydiator-core-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      605 2021-01-11 19:35:06.000000 pydiator-core-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-11 19:35:17.165312 pydiator-core-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-11 19:35:06.000000 pydiator-core-1.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3238 2021-01-11 19:35:06.000000 pydiator-core-1.0.8/tests/base_test_case.py
--rw-r--r--   0 runner    (1001) docker     (116)     1620 2021-01-11 19:35:06.000000 pydiator-core-1.0.8/tests/test_default_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (116)     5287 2021-01-11 19:35:06.000000 pydiator-core-1.0.8/tests/test_mediator_container.py
--rw-r--r--   0 runner    (1001) docker     (116)     7700 2021-01-11 19:35:06.000000 pydiator-core-1.0.8/tests/test_mediatr.py
--rw-r--r--   0 runner    (1001) docker     (116)     2619 2021-01-11 19:35:06.000000 pydiator-core-1.0.8/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (116)     1142 2021-01-11 19:35:06.000000 pydiator-core-1.0.8/tests/test_serializer_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-12 19:52:35.647567 pydiator-core-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)     8064 2021-01-12 19:52:35.647567 pydiator-core-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     6171 2021-01-12 19:52:24.000000 pydiator-core-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-12 19:52:35.647567 pydiator-core-1.0.9/pydiator_core/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-12 19:52:24.000000 pydiator-core-1.0.9/pydiator_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      935 2021-01-12 19:52:24.000000 pydiator-core-1.0.9/pydiator_core/default_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3010 2021-01-12 19:52:24.000000 pydiator-core-1.0.9/pydiator_core/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (116)      626 2021-01-12 19:52:24.000000 pydiator-core-1.0.9/pydiator_core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2148 2021-01-12 19:52:24.000000 pydiator-core-1.0.9/pydiator_core/mediatr.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2046 2021-01-12 19:52:24.000000 pydiator-core-1.0.9/pydiator_core/mediatr_container.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-12 19:52:35.647567 pydiator-core-1.0.9/pydiator_core/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-12 19:52:24.000000 pydiator-core-1.0.9/pydiator_core/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2288 2021-01-12 19:52:24.000000 pydiator-core-1.0.9/pydiator_core/pipelines/cache_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1268 2021-01-12 19:52:24.000000 pydiator-core-1.0.9/pydiator_core/pipelines/log_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1852 2021-01-12 19:52:24.000000 pydiator-core-1.0.9/pydiator_core/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-12 19:52:35.647567 pydiator-core-1.0.9/pydiator_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     8064 2021-01-12 19:52:35.000000 pydiator-core-1.0.9/pydiator_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      670 2021-01-12 19:52:35.000000 pydiator-core-1.0.9/pydiator_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-12 19:52:35.000000 pydiator-core-1.0.9/pydiator_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       20 2021-01-12 19:52:35.000000 pydiator-core-1.0.9/pydiator_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-12 19:52:35.647567 pydiator-core-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      605 2021-01-12 19:52:24.000000 pydiator-core-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-12 19:52:35.647567 pydiator-core-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-12 19:52:24.000000 pydiator-core-1.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3358 2021-01-12 19:52:24.000000 pydiator-core-1.0.9/tests/base_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2039 2021-01-12 19:52:24.000000 pydiator-core-1.0.9/tests/test_default_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5287 2021-01-12 19:52:24.000000 pydiator-core-1.0.9/tests/test_mediator_container.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7700 2021-01-12 19:52:24.000000 pydiator-core-1.0.9/tests/test_mediatr.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2619 2021-01-12 19:52:24.000000 pydiator-core-1.0.9/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1142 2021-01-12 19:52:24.000000 pydiator-core-1.0.9/tests/test_serializer_factory.py
```

### Comparing `pydiator-core-1.0.8/PKG-INFO` & `pydiator-core-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydiator-core
-Version: 1.0.8
+Version: 1.0.9
 Summary: Pydiator
 Home-page: https://github.com/ozgurkara/pydiator-core
 Author: Özgür Kara
 Author-email: ozgurkara85@gmail.com
 License: UNKNOWN
 Description: 
         [![](https://img.shields.io/pypi/pyversions/pydiator-core.svg)](https://pypi.org/project/pydiator-core/) ![example event parameter](https://github.com/ozgurkara/pydiator-core/workflows/CI/badge.svg) [![Coverage Status](https://coveralls.io/repos/github/ozgurkara/pydiator-core/badge.svg?branch=master)](https://coveralls.io/github/ozgurkara/pydiator-core?branch=master)  [![](https://img.shields.io/pypi/wheel/pydiator-core.svg)](https://pypi.org/project/pydiator-core/) [![](https://img.shields.io/pypi/format/pydiator-core.svg)](https://pypi.org/project/pydiator-core/)
@@ -131,15 +131,15 @@
                 container = MediatrContainer()        
                 container.register_pipeline(LogPipeline())
                 #container.register_pipeline(xPipeline())
                 pydiator.ready(container=container)
         ````
         <br/>
         
-        ***How can you write custom pipeline?***
+        ***How can you write a custom pipeline?***
            * Every pipeline  should be inherited ***BasePipeline***
            * Sample pipeline
         ```python
             class SamplePipeline(BasePipeline):
                 def __init__(self):
                     pass
             
@@ -151,33 +151,33 @@
             
                     # after executed next pipeline and use case            
         
                     return response
         ```   
         
         
-        # How to use the publisher subscriber feature
+        # How to use the notification-subscriber feature
         
-        ***What is the observer feature?***
+        ***What is the notification-subscriber feature?***
         
         This feature runs as pub-sub design pattern.
         
         **What is the pub-sub pattern?**
         
         publish-subscribe is a messaging pattern where senders of messages, called publishers, do not program the messages to be sent directly to specific receivers, called subscribers, but instead, categorize published messages into classes without knowledge of which subscribers if any, there may be. Similarly, subscribers express interest in one or more classes and only receive messages that are of interest, without knowledge of which publishers, if any, there are.
         <br/>
         
         **How to use this pattern with the pydiator?**
         
-        You can see the details that via this link https://github.com/ozgurkara/pydiator-core/blob/master/examples/pub_sub.py
+        You can see the details that via this link https://github.com/ozgurkara/pydiator-core/blob/master/examples/notification.py
         
         ```python
         def set_up_pydiator():
             container = MediatrContainer()
-            container.register_notification(SamplePublisherRequest, [Sample1Subscriber(), Sample2Subscriber(),
+            container.register_notification(SampleNotification, [Sample1Subscriber(), Sample2Subscriber(),
                                                                      Sample3Subscriber()])
             pydiator.ready(container=container)
         
         if __name__ == "__main__":
             set_up_pydiator()
             loop = asyncio.new_event_loop()
             loop.run_until_complete(pydiator.publish(SamplePublisherRequest(id=1)))
```

### Comparing `pydiator-core-1.0.8/README.md` & `pydiator-core-1.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         container = MediatrContainer()        
         container.register_pipeline(LogPipeline())
         #container.register_pipeline(xPipeline())
         pydiator.ready(container=container)
 ````
 <br/>
 
-***How can you write custom pipeline?***
+***How can you write a custom pipeline?***
    * Every pipeline  should be inherited ***BasePipeline***
    * Sample pipeline
 ```python
     class SamplePipeline(BasePipeline):
         def __init__(self):
             pass
     
@@ -143,33 +143,33 @@
     
             # after executed next pipeline and use case            
 
             return response
 ```   
 
 
-# How to use the publisher subscriber feature
+# How to use the notification-subscriber feature
 
-***What is the observer feature?***
+***What is the notification-subscriber feature?***
 
 This feature runs as pub-sub design pattern.
 
 **What is the pub-sub pattern?**
 
 publish-subscribe is a messaging pattern where senders of messages, called publishers, do not program the messages to be sent directly to specific receivers, called subscribers, but instead, categorize published messages into classes without knowledge of which subscribers if any, there may be. Similarly, subscribers express interest in one or more classes and only receive messages that are of interest, without knowledge of which publishers, if any, there are.
 <br/>
 
 **How to use this pattern with the pydiator?**
 
-You can see the details that via this link https://github.com/ozgurkara/pydiator-core/blob/master/examples/pub_sub.py
+You can see the details that via this link https://github.com/ozgurkara/pydiator-core/blob/master/examples/notification.py
 
 ```python
 def set_up_pydiator():
     container = MediatrContainer()
-    container.register_notification(SamplePublisherRequest, [Sample1Subscriber(), Sample2Subscriber(),
+    container.register_notification(SampleNotification, [Sample1Subscriber(), Sample2Subscriber(),
                                                              Sample3Subscriber()])
     pydiator.ready(container=container)
 
 if __name__ == "__main__":
     set_up_pydiator()
     loop = asyncio.new_event_loop()
     loop.run_until_complete(pydiator.publish(SamplePublisherRequest(id=1)))
```

### Comparing `pydiator-core-1.0.8/pydiator_core/default_pipeline.py` & `pydiator-core-1.0.9/pydiator_core/default_pipeline.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import inspect
+
 from pydiator_core.interfaces import BaseRequest, BasePipeline
 from pydiator_core.mediatr_container import BaseMediatrContainer
 
 
 class DefaultPipeline(BasePipeline):
     def __init__(self, mediatr_container: BaseMediatrContainer):
         self.mediatr_container = mediatr_container
@@ -12,8 +14,12 @@
         if handler is None:
             raise Exception(f"handler_not_found_for_request_:{req_type_name}")
 
         handle_func = getattr(handler, "handle", None)
         if not callable(handle_func):
             raise Exception("handle_function_has_not_found_in_handler")
 
+        is_async = inspect.iscoroutinefunction(handler.handle)
+        if not is_async:
+            return handler.handle(req)
+
         return await handler.handle(req)
```

### Comparing `pydiator-core-1.0.8/pydiator_core/interfaces.py` & `pydiator-core-1.0.9/pydiator_core/interfaces.py`

 * *Files identical despite different names*

### Comparing `pydiator-core-1.0.8/pydiator_core/logger.py` & `pydiator-core-1.0.9/pydiator_core/logger.py`

 * *Files identical despite different names*

### Comparing `pydiator-core-1.0.8/pydiator_core/mediatr.py` & `pydiator-core-1.0.9/pydiator_core/mediatr.py`

 * *Files identical despite different names*

### Comparing `pydiator-core-1.0.8/pydiator_core/mediatr_container.py` & `pydiator-core-1.0.9/pydiator_core/mediatr_container.py`

 * *Files identical despite different names*

### Comparing `pydiator-core-1.0.8/pydiator_core/pipelines/cache_pipeline.py` & `pydiator-core-1.0.9/pydiator_core/pipelines/cache_pipeline.py`

 * *Files identical despite different names*

### Comparing `pydiator-core-1.0.8/pydiator_core/pipelines/log_pipeline.py` & `pydiator-core-1.0.9/pydiator_core/pipelines/log_pipeline.py`

 * *Files identical despite different names*

### Comparing `pydiator-core-1.0.8/pydiator_core/serializer.py` & `pydiator-core-1.0.9/pydiator_core/serializer.py`

 * *Files identical despite different names*

### Comparing `pydiator-core-1.0.8/pydiator_core.egg-info/PKG-INFO` & `pydiator-core-1.0.9/pydiator_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydiator-core
-Version: 1.0.8
+Version: 1.0.9
 Summary: Pydiator
 Home-page: https://github.com/ozgurkara/pydiator-core
 Author: Özgür Kara
 Author-email: ozgurkara85@gmail.com
 License: UNKNOWN
 Description: 
         [![](https://img.shields.io/pypi/pyversions/pydiator-core.svg)](https://pypi.org/project/pydiator-core/) ![example event parameter](https://github.com/ozgurkara/pydiator-core/workflows/CI/badge.svg) [![Coverage Status](https://coveralls.io/repos/github/ozgurkara/pydiator-core/badge.svg?branch=master)](https://coveralls.io/github/ozgurkara/pydiator-core?branch=master)  [![](https://img.shields.io/pypi/wheel/pydiator-core.svg)](https://pypi.org/project/pydiator-core/) [![](https://img.shields.io/pypi/format/pydiator-core.svg)](https://pypi.org/project/pydiator-core/)
@@ -131,15 +131,15 @@
                 container = MediatrContainer()        
                 container.register_pipeline(LogPipeline())
                 #container.register_pipeline(xPipeline())
                 pydiator.ready(container=container)
         ````
         <br/>
         
-        ***How can you write custom pipeline?***
+        ***How can you write a custom pipeline?***
            * Every pipeline  should be inherited ***BasePipeline***
            * Sample pipeline
         ```python
             class SamplePipeline(BasePipeline):
                 def __init__(self):
                     pass
             
@@ -151,33 +151,33 @@
             
                     # after executed next pipeline and use case            
         
                     return response
         ```   
         
         
-        # How to use the publisher subscriber feature
+        # How to use the notification-subscriber feature
         
-        ***What is the observer feature?***
+        ***What is the notification-subscriber feature?***
         
         This feature runs as pub-sub design pattern.
         
         **What is the pub-sub pattern?**
         
         publish-subscribe is a messaging pattern where senders of messages, called publishers, do not program the messages to be sent directly to specific receivers, called subscribers, but instead, categorize published messages into classes without knowledge of which subscribers if any, there may be. Similarly, subscribers express interest in one or more classes and only receive messages that are of interest, without knowledge of which publishers, if any, there are.
         <br/>
         
         **How to use this pattern with the pydiator?**
         
-        You can see the details that via this link https://github.com/ozgurkara/pydiator-core/blob/master/examples/pub_sub.py
+        You can see the details that via this link https://github.com/ozgurkara/pydiator-core/blob/master/examples/notification.py
         
         ```python
         def set_up_pydiator():
             container = MediatrContainer()
-            container.register_notification(SamplePublisherRequest, [Sample1Subscriber(), Sample2Subscriber(),
+            container.register_notification(SampleNotification, [Sample1Subscriber(), Sample2Subscriber(),
                                                                      Sample3Subscriber()])
             pydiator.ready(container=container)
         
         if __name__ == "__main__":
             set_up_pydiator()
             loop = asyncio.new_event_loop()
             loop.run_until_complete(pydiator.publish(SamplePublisherRequest(id=1)))
```

### Comparing `pydiator-core-1.0.8/pydiator_core.egg-info/SOURCES.txt` & `pydiator-core-1.0.9/pydiator_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydiator-core-1.0.8/setup.py` & `pydiator-core-1.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pydiator-core",
-    version="1.0.8",
+    version="1.0.9",
     author="Özgür Kara",
     author_email="ozgurkara85@gmail.com",
     description="Pydiator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ozgurkara/pydiator-core",
     packages=setuptools.find_packages(),
```

### Comparing `pydiator-core-1.0.8/tests/base_test_case.py` & `pydiator-core-1.0.9/tests/base_test_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,19 @@
 
 
 class TestHandler(BaseHandler):
     async def handle(self, req: BaseRequest):
         return TestResponse(success=True)
 
 
+class TestSyncHandler(BaseHandler):
+    def handle(self, req: BaseRequest):
+        return TestResponse(success=True)
+
+
 class TestPipeline(BasePipeline):
     def __init__(self, response_success):
         self.response_success = response_success
 
     async def handle(self, req: BaseRequest) -> object:
         return TestResponse(success=self.response_success)
```

### Comparing `pydiator-core-1.0.8/tests/test_default_pipeline.py` & `pydiator-core-1.0.9/tests/test_default_pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest import mock
 
 from pydiator_core.default_pipeline import DefaultPipeline
 from pydiator_core.interfaces import BaseResponse
 from pydiator_core.mediatr_container import MediatrContainer
-from tests.base_test_case import BaseTestCase, TestRequest, TestHandler
+from tests.base_test_case import BaseTestCase, TestRequest, TestHandler, TestSyncHandler
 
 
 class TestDefaultPipeline(BaseTestCase):
     def setUp(self):
         pass
 
     def test_handle_return_exception_when_handler_is_not(self):
@@ -41,7 +41,19 @@
         self.pipeline = DefaultPipeline(container)
 
         # When
         response = self.async_loop(self.pipeline.handle(req=TestRequest()))
 
         # Then
         assert isinstance(response, BaseResponse)
+
+    def test_handle_return_handle_response_when_handle_is_sync(self):
+        # Given
+        container = MediatrContainer()
+        container.register_request(TestRequest, TestSyncHandler())
+        self.pipeline = DefaultPipeline(container)
+
+        # When
+        response = self.async_loop(self.pipeline.handle(req=TestRequest()))
+
+        # Then
+        assert isinstance(response, BaseResponse)
```

### Comparing `pydiator-core-1.0.8/tests/test_mediator_container.py` & `pydiator-core-1.0.9/tests/test_mediator_container.py`

 * *Files identical despite different names*

### Comparing `pydiator-core-1.0.8/tests/test_mediatr.py` & `pydiator-core-1.0.9/tests/test_mediatr.py`

 * *Files identical despite different names*

### Comparing `pydiator-core-1.0.8/tests/test_serializer.py` & `pydiator-core-1.0.9/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `pydiator-core-1.0.8/tests/test_serializer_factory.py` & `pydiator-core-1.0.9/tests/test_serializer_factory.py`

 * *Files identical despite different names*

