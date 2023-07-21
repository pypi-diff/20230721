# Comparing `tmp/zmq_tubes-1.8.0.tar.gz` & `tmp/zmq_tubes-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zmq_tubes-1.8.0.tar", max compression
+gzip compressed data, was "zmq_tubes-1.9.0.tar", max compression
```

## Comparing `zmq_tubes-1.8.0.tar` & `zmq_tubes-1.9.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     7951 2022-10-12 11:05:03.730297 zmq_tubes-1.8.0/README.md
--rw-r--r--   0        0        0      910 2022-10-12 11:05:18.955571 zmq_tubes-1.8.0/pyproject.toml
--rw-r--r--   0        0        0      198 2022-10-12 11:05:03.734297 zmq_tubes-1.8.0/zmq_tubes/__init__.py
--rw-r--r--   0        0        0    23713 2022-10-12 11:05:03.734297 zmq_tubes-1.8.0/zmq_tubes/manager.py
--rw-r--r--   0        0        0     3392 2022-10-12 11:05:03.734297 zmq_tubes-1.8.0/zmq_tubes/matcher.py
--rw-r--r--   0        0        0    10185 2022-10-12 11:05:03.734297 zmq_tubes-1.8.0/zmq_tubes/threads.py
--rw-r--r--   0        0        0     8998 1970-01-01 00:00:00.000000 zmq_tubes-1.8.0/setup.py
--rw-r--r--   0        0        0     8925 1970-01-01 00:00:00.000000 zmq_tubes-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     7951 2022-10-12 14:03:14.327857 zmq_tubes-1.9.0/README.md
+-rw-r--r--   0        0        0      910 2022-10-12 14:03:22.804057 zmq_tubes-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      198 2022-10-12 14:03:14.327857 zmq_tubes-1.9.0/zmq_tubes/__init__.py
+-rw-r--r--   0        0        0    23826 2022-10-12 14:03:14.331857 zmq_tubes-1.9.0/zmq_tubes/manager.py
+-rw-r--r--   0        0        0     3392 2022-10-12 14:03:14.331857 zmq_tubes-1.9.0/zmq_tubes/matcher.py
+-rw-r--r--   0        0        0    10286 2022-10-12 14:03:14.331857 zmq_tubes-1.9.0/zmq_tubes/threads.py
+-rw-r--r--   0        0        0     8998 1970-01-01 00:00:00.000000 zmq_tubes-1.9.0/setup.py
+-rw-r--r--   0        0        0     8925 1970-01-01 00:00:00.000000 zmq_tubes-1.9.0/PKG-INFO
```

### Comparing `zmq_tubes-1.8.0/README.md` & `zmq_tubes-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `zmq_tubes-1.8.0/pyproject.toml` & `zmq_tubes-1.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zmq_tubes"
-version = "1.8.0"
+version = "1.9.0"
 license = "MIT"
 readme = "README.md"
 description = "Wrapper for ZMQ comunication."
 authors = ["Martin Korbel <mkorbel@alps.cz>"]
 homepage = "https://github.com/calcite/zmq_tubes"
 repository = "https://github.com/calcite/zmq_tubes"
 documentation = "https://github.com/calcite/zmq_tubes"
```

### Comparing `zmq_tubes-1.8.0/zmq_tubes/manager.py` & `zmq_tubes-1.9.0/zmq_tubes/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -562,21 +562,22 @@
             tube = self.get_tube_by_topic(topic, [zmq.DEALER])
             if not tube:
                 raise TubeTopicNotConfigured(f'The topic "{topic}" is not '
                                              f'assigned to any Tube for '
                                              f'dealer.')
         tube.send(topic, payload)
 
-    async def request(self, topic: str, payload=None, timeout=30) \
-            -> TubeMessage:
+    async def request(self, topic: str, payload=None, timeout=30,
+                      post_send_callback=None) -> TubeMessage:
         tube = self.get_tube_by_topic(topic, [zmq.REQ])
         if not tube:
             raise TubeTopicNotConfigured(f'The topic "{topic}" is not assigned '
                                          f'to any Tube for request.')
-        res = await tube.request(topic, payload, timeout)
+        res = await tube.request(topic, payload, timeout=timeout,
+                                 post_send_callback=post_send_callback)
         return res
 
     def publish(self, topic: str, payload=None):
         """
         In the case with asyncio, the first message is very often lost.
         The workaround is to connect the tube manually as soon as possible.
         """
```

### Comparing `zmq_tubes-1.8.0/zmq_tubes/matcher.py` & `zmq_tubes-1.9.0/zmq_tubes/matcher.py`

 * *Files identical despite different names*

### Comparing `zmq_tubes-1.8.0/zmq_tubes/threads.py` & `zmq_tubes-1.9.0/zmq_tubes/threads.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,21 +148,22 @@
         self.connect()
         self.start()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.stop()
         self.close()
 
-    def request(self, topic: str, payload=None, timeout=30) \
-            -> TubeMessage:
+    def request(self, topic: str, payload=None, timeout=30,
+                post_send_callback=None) -> TubeMessage:
         tube = self.get_tube_by_topic(topic, [zmq.REQ])
         if not tube:
             raise TubeTopicNotConfigured(f'The topic "{topic}" is not assigned '
                                          f'to any Tube for request.')
-        res = tube.request(topic, payload, timeout)
+        res = tube.request(topic, payload, timeout=timeout,
+                           post_send_callback=post_send_callback)
         return res
 
     def stop(self):
         if self.__main_thread:
             self.__main_thread.stop()
 
     def start(self):
```

### Comparing `zmq_tubes-1.8.0/setup.py` & `zmq_tubes-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pyzmq']
 
 setup_kwargs = {
     'name': 'zmq-tubes',
-    'version': '1.8.0',
+    'version': '1.9.0',
     'description': 'Wrapper for ZMQ comunication.',
     'long_description': "[![PyPI](https://img.shields.io/pypi/v/zmq_tubes?color=green&style=plastic)](https://pypi.org/project/zmq-tubes/)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zmq_tubes?style=plastic)\n![License](https://img.shields.io/github/license/calcite/zmq_tubes?style=plastic)\n# ZMQ Tubes\n\nZMQ Tubes is a managing system for ZMQ communication. \nIt can manage many ZMQ sockets by one interface. \nThe whole system is hierarchical, based on topics \n(look at [MQTT topics](https://www.hivemq.com/blog/mqtt-essentials-part-5-mqtt-topics-best-practices/)).\n\n## Classes\n- **TubeMessage** - This class represents a request/response message. \n  Some types of tubes require a response in this format.\n- **Tube** - This class wraps a ZMQ socket. \n  It represents a connection between client and server.\n- **TubeNode** - This represents an application interface for communication via tubes.\n\n\n## Asyncio / Threading\nThe library support bot method. Asyncio from Python 3.7.\n\n```python\nfrom zmq_tubes import TubeNode, Tube            # Asyncio classes\nfrom zmq_tubes.threads import TubeNode, Tube    # Threads classes\n```\n\n\n## Usage:\n\n### Node definitions in yml file \nWe can define all tubes for one TubeNode by yml file. \n\n```yaml\n# test.yml\ntubes:\n  - name: Client REQ\n    addr:  ipc:///tmp/req.pipe      \n    tube_type: REQ\n    topics:\n      - foo/#\n      - +/bar\n  \n  - name: Client PUB\n    addr:  ipc:///tmp/pub.pipe      \n    tube_type: PUB\n    topics:\n      - foo/pub/#\n\n  - name: Server ROUTER\n    addr:  ipc:///tmp/router.pipe      \n    tube_type: ROUTER\n    server: yes\n    sockopts:\n      LINGER: 0\n    topics:\n      - server/#\n```\n\n```python\nimport asyncio\nimport yaml\nfrom zmq_tubes import TubeNode, TubeMessage\n\n\nasync def handler(request: TubeMessage):\n  print(request.payload)\n  return request.create_response('response')\n\n\nasync def run():\n  with open('test.yml', 'r+') as fd:\n    schema = yaml.safe_load(fd)\n  node = TubeNode(schema=schema)\n  node.register_handler('server/#', handler)\n  with node:\n      node.publish('foo/pub/test', 'message 1')\n      print(await node.request('foo/xxx', 'message 2'))\n\nasyncio.run(run())\n```\n\n\n\n\n### Request / Response\nThis is a simple scenario, the server processes the requests serially.\n#### Server:\n\n```python\nfrom zmq_tubes import Tube, TubeNode, TubeMessage\n\n\nasync def handler(request: TubeMessage):\n  print(request.payload)\n  return 'answer'\n  # or return request.create_response('response')\n\n\ntube = Tube(\n  name='Server',\n  addr='ipc:///tmp/req_resp.pipe',\n  server=True,\n  tube_type='REP'\n)\n\nnode = TubeNode()\nnode.register_tube(tube, 'test/#')\nnode.register_handler('test/#', handler)\nawait node.start()\n\n# output: 'question'\n```\n\n#### Client:\n\n```python\nfrom zmq_tubes import Tube, TubeNode\n\ntube = Tube(\n  name='Client',\n  addr='ipc:///tmp/req_resp.pipe',\n  tube_type='REQ'\n)\n\nnode = TubeNode()\nnode.register_tube(tube, 'test/#')\nresponse = await node.request('test/xxx', 'question')\nprint(response.payload)\n# output: 'answer'\n```\n\n\n\n\n### Subscribe / Publisher\n#### Server:\n\n```python\nfrom zmq_tubes import Tube, TubeNode, TubeMessage\n\n\nasync def handler(request: TubeMessage):\n  print(request.payload)\n\n\ntube = Tube(\n  name='Server',\n  addr='ipc:///tmp/sub_pub.pipe',\n  server=True,\n  tube_type='SUB'\n)\n\nnode = TubeNode()\nnode.register_tube(tube, 'test/#')\nnode.register_handler('test/#', handler)\nawait node.start()\n# output: 'message'\n```\n\n#### Client:\n\n```python\nfrom zmq_tubes import Tube, TubeNode\n\ntube = Tube(\n  name='Client',\n  addr='ipc:///tmp/sub_pub.pipe',\n  tube_type='PUB'\n)\n# In the case of publishing, the first message is very often\n# lost. The workaround is to connect the tube manually as soon as possible.\ntube.connect()\n\nnode = TubeNode()\nnode.register_tube(tube, 'test/#')\nnode.publish('test/xxx', 'message')        \n```\n\n\n\n\n### Request / Router\nThe server is asynchronous. It means it is able to process \nmore requests at the same time.\n\n#### Server:\n\n```python\nimport asyncio\nfrom zmq_tubes import Tube, TubeNode, TubeMessage\n\n\nasync def handler(request: TubeMessage):\n  print(request.payload)\n  if request.payload == 'wait':\n    await asyncio.sleep(10)\n  return request.create_response(request.payload)\n\n\ntube = Tube(\n  name='Server',\n  addr='ipc:///tmp/req_router.pipe',\n  server=True,\n  tube_type='ROUTER'\n)\n\nnode = TubeNode()\nnode.register_tube(tube, 'test/#')\nnode.register_handler('test/#', handler)\nawait node.start()\n# output: 'wait'\n# output: 'message'\n```\n\n#### Client:\n\n```python\nimport asyncio\nfrom zmq_tubes import Tube, TubeNode\n\ntube = Tube(\n  name='Client',\n  addr='ipc:///tmp/req_router.pipe',\n  tube_type='REQ'\n)\n\n\nasync def task(node, text):\n  print(await node.request('test/xxx', text))\n\n\nnode = TubeNode()\nnode.register_tube(tube, 'test/#')\nasyncio.create_task(task(node, 'wait'))\nasyncio.create_task(task(node, 'message'))\n# output: 'message'\n# output: 'wait'\n```\n\n\n\n\n### Dealer / Response\nThe client is asynchronous. It means it is able to send \nmore requests at the same time.\n\n#### Server:\n\n```python\nfrom zmq_tubes import Tube, TubeNode, TubeMessage\n\n\nasync def handler(request: TubeMessage):\n  print(request.payload)\n  return 'response'\n  # or return requset.create_response('response')\n\n\ntube = Tube(\n  name='Server',\n  addr='ipc:///tmp/dealer_resp.pipe',\n  server=True,\n  tube_type='REP'\n)\n\nnode = TubeNode()\nnode.register_tube(tube, 'test/#')\nnode.register_handler('test/#', handler)\nawait node.start()\n# output: 'message'\n```\n\n#### Client:\n\n```python\nfrom zmq_tubes import Tube, TubeNode, TubeMessage\n\ntube = Tube(\n  name='Client',\n  addr='ipc:///tmp/dealer_resp.pipe',\n  tube_type='DEALER'\n)\n\n\nasync def handler(response: TubeMessage):\n  print(response.payload)\n\n\nnode = TubeNode()\nnode.register_tube(tube, 'test/#')\nnode.register_handler('test/#', handler)\n\nnode.send('test/xxx', 'message')\n\n# output: 'response'\n```\n\n\n\n### Dealer / Router\nThe client and server are asynchronous. It means it is able to send and process \nmore requests/responses at the same time.\n\n#### Server:\n\n```python\nimport asyncio\nfrom zmq_tubes import Tube, TubeNode, TubeMessage\n\n\nasync def handler(request: TubeMessage):\n  print(request.payload)\n  if request.payload == 'wait':\n    await asyncio.sleep(10)\n  return request.create_response(request.payload)\n\n\ntube = Tube(\n  name='Server',\n  addr='ipc:///tmp/dealer_router.pipe',\n  server=True,\n  tube_type='ROUTER'\n)\n\nnode = TubeNode()\nnode.register_tube(tube, 'test/#')\nnode.register_handler('test/#', handler)\nawait node.start()\n# output: 'wait'\n# output: 'message'\n```\n\n#### Client:\n\n```python\nfrom zmq_tubes import Tube, TubeNode, TubeMessage\n\ntube = Tube(\n  name='Client',\n  addr='ipc:///tmp/dealer_router.pipe',\n  tube_type='DEALER'\n)\n\n\nasync def handler(response: TubeMessage):\n  print(response.payload)\n\n\nnode = TubeNode()\nnode.register_tube(tube, 'test/#')\nnode.register_handler('test/#', handler)\n\nnode.send('test/xxx', 'wait')\nnode.send('test/xxx', 'message')\n\n# output: 'message'\n# output: 'wait'\n```\n\n\n\n### Dealer / Dealer\nThe client and server are asynchronous. It means it is able to send and process \nmore requests/responses at the same time.\n\n#### Server:\n\n```python\nfrom zmq_tubes import Tube, TubeNode, TubeMessage\n\ntube = Tube(\n  name='Server',\n  addr='ipc:///tmp/dealer_dealer.pipe',\n  server=True,\n  tube_type='DEALER'\n)\n\n\nasync def handler(response: TubeMessage):\n  print(response.payload)\n\n\nnode = TubeNode()\nnode.register_tube(tube, 'test/#')\nnode.register_handler('test/#', handler)\n\nnode.send('test/xxx', 'message from server')\n# output: 'message from client'\n```\n\n#### Client:\n\n```python\nfrom zmq_tubes import Tube, TubeNode, TubeMessage\n\ntube = Tube(\n  name='Client',\n  addr='ipc:///tmp/dealer_dealer.pipe',\n  tube_type='DEALER'\n)\n\n\nasync def handler(response: TubeMessage):\n  print(response.payload)\n\n\nnode = TubeNode()\nnode.register_tube(tube, 'test/#')\nnode.register_handler('test/#', handler)\n\nnode.send('test/xxx', 'message from client')\n# output: 'message from server'\n```\n",
     'author': 'Martin Korbel',
     'author_email': 'mkorbel@alps.cz',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/calcite/zmq_tubes',
```

### Comparing `zmq_tubes-1.8.0/PKG-INFO` & `zmq_tubes-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zmq-tubes
-Version: 1.8.0
+Version: 1.9.0
 Summary: Wrapper for ZMQ comunication.
 Home-page: https://github.com/calcite/zmq_tubes
 License: MIT
 Keywords: zmq,mqtt,tubes,zmq_tubes
 Author: Martin Korbel
 Author-email: mkorbel@alps.cz
 Requires-Python: >=3.6,<4.0
```

