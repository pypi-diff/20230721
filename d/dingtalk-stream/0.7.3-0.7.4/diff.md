# Comparing `tmp/dingtalk-stream-0.7.3.tar.gz` & `tmp/dingtalk-stream-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingtalk-stream-0.7.3.tar", last modified: Thu Jul 20 08:21:27 2023, max compression
+gzip compressed data, was "dingtalk-stream-0.7.4.tar", last modified: Fri Jul 21 02:07:39 2023, max compression
```

## Comparing `dingtalk-stream-0.7.3.tar` & `dingtalk-stream-0.7.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:21:27.139819 dingtalk-stream-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-20 08:21:27.139819 dingtalk-stream-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:21:27.139819 dingtalk-stream-0.7.3/dingtalk_stream/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/card_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/card_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/card_replier.py
--rw-r--r--   0 runner    (1001) docker     (123)    25086 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/interactive_card.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:21:27.139819 dingtalk-stream-0.7.3/dingtalk_stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-20 08:21:27.000000 dingtalk-stream-0.7.3/dingtalk_stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-20 08:21:27.000000 dingtalk-stream-0.7.3/dingtalk_stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:21:27.000000 dingtalk-stream-0.7.3/dingtalk_stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-20 08:21:27.000000 dingtalk-stream-0.7.3/dingtalk_stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 08:21:27.000000 dingtalk-stream-0.7.3/dingtalk_stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:21:27.139819 dingtalk-stream-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:07:39.927550 dingtalk-stream-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-21 02:07:39.927550 dingtalk-stream-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:07:39.927550 dingtalk-stream-0.7.4/dingtalk_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/card_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/card_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/card_replier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25086 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/interactive_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/dingtalk_stream/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:07:39.927550 dingtalk-stream-0.7.4/dingtalk_stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-21 02:07:39.000000 dingtalk-stream-0.7.4/dingtalk_stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-21 02:07:39.000000 dingtalk-stream-0.7.4/dingtalk_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 02:07:39.000000 dingtalk-stream-0.7.4/dingtalk_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-21 02:07:39.000000 dingtalk-stream-0.7.4/dingtalk_stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 02:07:39.000000 dingtalk-stream-0.7.4/dingtalk_stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 02:07:39.927550 dingtalk-stream-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-21 02:07:38.000000 dingtalk-stream-0.7.4/setup.py
```

### Comparing `dingtalk-stream-0.7.3/LICENSE` & `dingtalk-stream-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.3/PKG-INFO` & `dingtalk-stream-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.7.3
+Version: 0.7.4
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.7.3/README.md` & `dingtalk-stream-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.3/dingtalk_stream/__init__.py` & `dingtalk-stream-0.7.4/dingtalk_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.3/dingtalk_stream/card_callback.py` & `dingtalk-stream-0.7.4/dingtalk_stream/card_callback.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.3/dingtalk_stream/card_instance.py` & `dingtalk-stream-0.7.4/dingtalk_stream/card_instance.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.3/dingtalk_stream/card_replier.py` & `dingtalk-stream-0.7.4/dingtalk_stream/card_replier.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.3/dingtalk_stream/chatbot.py` & `dingtalk-stream-0.7.4/dingtalk_stream/chatbot.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.3/dingtalk_stream/frames.py` & `dingtalk-stream-0.7.4/dingtalk_stream/frames.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.3/dingtalk_stream/handlers.py` & `dingtalk-stream-0.7.4/dingtalk_stream/handlers.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.3/dingtalk_stream/interactive_card.py` & `dingtalk-stream-0.7.4/dingtalk_stream/interactive_card.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.3/dingtalk_stream/stream.py` & `dingtalk-stream-0.7.4/dingtalk_stream/stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import logging
 import platform
 import time
 import urllib.error
 import urllib.parse
 import urllib.request
 import requests
+import socket
 
 import websockets
 
 from .credential import Credential
 from .handlers import CallbackHandler
 from .handlers import EventHandler
 from .handlers import SystemHandler
@@ -140,27 +141,42 @@
             topics.append({'type': 'EVENT', 'topic': '*'})
         for topic in self.callback_handler_map.keys():
             topics.append({'type': 'CALLBACK', 'topic': topic})
         request_body = json.dumps({
             'clientId': self.credential.client_id,
             'clientSecret': self.credential.client_secret,
             'subscriptions': topics,
+            'localIp': self.get_host_ip()
         }).encode('utf-8')
 
         try:
             response = requests.post(DingTalkStreamClient.OPEN_CONNECTION_API,
                                      headers=request_headers,
                                      data=request_body)
             http_body = response.json()
             response.raise_for_status()
         except Exception as e:
             self.logger.error("open connection failed, error=%s, response.body=%s", e, http_body)
             return None
         return response.json()
 
+    def get_host_ip(self):
+        """
+        查询本机ip地址
+        :return: ip
+        """
+        ip = ""
+        try:
+            s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+            s.connect(('8.8.8.8', 80))
+            ip = s.getsockname()[0]
+        finally:
+            s.close()
+            return ip
+
     def reset_access_token(self):
         """ reset token if open api return 401 """
         self._access_token = {}
 
     def get_access_token(self):
         now = int(time.time())
         if self._access_token and now < self._access_token['expireTime']:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dingtalk-stream-0.7.3/dingtalk_stream.egg-info/PKG-INFO` & `dingtalk-stream-0.7.4/dingtalk_stream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.7.3
+Version: 0.7.4
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.7.3/dingtalk_stream.egg-info/SOURCES.txt` & `dingtalk-stream-0.7.4/dingtalk_stream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.3/setup.py` & `dingtalk-stream-0.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='dingtalk-stream',
-    version='0.7.3',
+    version='0.7.4',
     description='A Python library for sending messages to DingTalk chatbot',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/open-dingtalk/dingtalk-stream-sdk-python',
     author='Ke Jie',
     author_email='jinxi.kj@alibaba-inc.com',
     license='MIT',
```

