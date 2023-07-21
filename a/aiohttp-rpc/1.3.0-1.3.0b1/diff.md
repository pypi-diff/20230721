# Comparing `tmp/aiohttp-rpc-1.3.0.tar.gz` & `tmp/aiohttp-rpc-1.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp-rpc-1.3.0.tar", last modified: Fri Jul 21 18:56:32 2023, max compression
+gzip compressed data, was "aiohttp-rpc-1.3.0b1.tar", last modified: Sat Jul  8 06:30:08 2023, max compression
```

## Comparing `aiohttp-rpc-1.3.0.tar` & `aiohttp-rpc-1.3.0b1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-21 18:56:32.117183 aiohttp-rpc-1.3.0/
--rwxrwxrwx   0 michael   (1000) michael   (1000)     1071 2022-06-22 04:31:16.000000 aiohttp-rpc-1.3.0/LICENSE.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)    14493 2023-07-21 18:56:32.117183 aiohttp-rpc-1.3.0/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)    13133 2023-07-21 18:54:53.000000 aiohttp-rpc-1.3.0/README.md
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-21 18:56:32.109183 aiohttp-rpc-1.3.0/aiohttp_rpc/
--rwxrwxrwx   0 michael   (1000) michael   (1000)      376 2022-07-08 14:39:35.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-21 18:56:32.113183 aiohttp-rpc-1.3.0/aiohttp_rpc/client/
--rwxrwxrwx   0 michael   (1000) michael   (1000)      122 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/client/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     6157 2023-07-08 06:31:56.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/client/base.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)     1832 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/client/http.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)        0 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/client/py.typed
--rw-rw-r--   0 michael   (1000) michael   (1000)    11246 2023-07-08 06:31:56.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/client/websocket.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)      157 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/constants.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)      585 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/decorators.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)     2497 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/errors.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)     2461 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/middlewares.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-21 18:56:32.113183 aiohttp-rpc-1.3.0/aiohttp_rpc/protocol/
--rwxrwxrwx   0 michael   (1000) michael   (1000)      126 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/protocol/__init__.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)     5178 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/protocol/method.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)        0 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/protocol/py.typed
--rwxrwxrwx   0 michael   (1000) michael   (1000)     3640 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/protocol/request.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)     3940 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/protocol/response.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)        0 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/py.typed
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-21 18:56:32.113183 aiohttp-rpc-1.3.0/aiohttp_rpc/server/
--rwxrwxrwx   0 michael   (1000) michael   (1000)      122 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/server/__init__.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)     6540 2023-03-23 19:05:25.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/server/base.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)      995 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/server/http.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)        0 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/server/py.typed
--rwxrwxrwx   0 michael   (1000) michael   (1000)     3408 2022-07-08 15:43:12.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/server/websocket.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)      946 2023-03-23 19:03:20.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/typedefs.py
--rwxrwxrwx   0 michael   (1000) michael   (1000)     3245 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0/aiohttp_rpc/utils.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-21 18:56:32.109183 aiohttp-rpc-1.3.0/aiohttp_rpc.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)    14493 2023-07-21 18:56:30.000000 aiohttp-rpc-1.3.0/aiohttp_rpc.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)      858 2023-07-21 18:56:32.000000 aiohttp-rpc-1.3.0/aiohttp_rpc.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-07-21 18:56:30.000000 aiohttp-rpc-1.3.0/aiohttp_rpc.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       14 2023-07-21 18:56:31.000000 aiohttp-rpc-1.3.0/aiohttp_rpc.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       12 2023-07-21 18:56:31.000000 aiohttp-rpc-1.3.0/aiohttp_rpc.egg-info/top_level.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)      437 2023-07-21 18:50:27.000000 aiohttp-rpc-1.3.0/pyproject.toml
--rw-rw-r--   0 michael   (1000) michael   (1000)       38 2023-07-21 18:56:32.117183 aiohttp-rpc-1.3.0/setup.cfg
--rwxrwxrwx   0 michael   (1000) michael   (1000)     2285 2023-07-21 18:50:27.000000 aiohttp-rpc-1.3.0/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-08 06:30:08.921718 aiohttp-rpc-1.3.0b1/
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     1071 2022-06-22 04:31:16.000000 aiohttp-rpc-1.3.0b1/LICENSE.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)    14495 2023-07-08 06:30:08.921718 aiohttp-rpc-1.3.0b1/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)    13133 2023-07-08 06:26:15.000000 aiohttp-rpc-1.3.0b1/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-08 06:30:08.917717 aiohttp-rpc-1.3.0b1/aiohttp_rpc/
+-rwxrwxrwx   0 michael   (1000) michael   (1000)      376 2022-07-08 14:39:35.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-08 06:30:08.917717 aiohttp-rpc-1.3.0b1/aiohttp_rpc/client/
+-rwxrwxrwx   0 michael   (1000) michael   (1000)      122 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/client/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6158 2023-07-08 06:26:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/client/base.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     1832 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/client/http.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)        0 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/client/py.typed
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8797 2023-07-08 06:26:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/client/websocket.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)      157 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/constants.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)      585 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/decorators.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     2497 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/errors.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     2461 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/middlewares.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-08 06:30:08.921718 aiohttp-rpc-1.3.0b1/aiohttp_rpc/protocol/
+-rwxrwxrwx   0 michael   (1000) michael   (1000)      126 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/protocol/__init__.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     5178 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/protocol/method.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)        0 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/protocol/py.typed
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     3640 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/protocol/request.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     3940 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/protocol/response.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)        0 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/py.typed
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-08 06:30:08.921718 aiohttp-rpc-1.3.0b1/aiohttp_rpc/server/
+-rwxrwxrwx   0 michael   (1000) michael   (1000)      122 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/server/__init__.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     6540 2023-03-23 19:05:25.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/server/base.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)      995 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/server/http.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)        0 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/server/py.typed
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     3408 2022-07-08 15:43:12.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/server/websocket.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)      946 2023-03-23 19:03:20.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/typedefs.py
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     3245 2022-06-22 04:31:15.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc/utils.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-08 06:30:08.917717 aiohttp-rpc-1.3.0b1/aiohttp_rpc.egg-info/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    14495 2023-07-08 06:30:08.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)      858 2023-07-08 06:30:08.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-07-08 06:30:08.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       14 2023-07-08 06:30:08.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       12 2023-07-08 06:30:08.000000 aiohttp-rpc-1.3.0b1/aiohttp_rpc.egg-info/top_level.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)      438 2023-07-08 06:28:39.000000 aiohttp-rpc-1.3.0b1/pyproject.toml
+-rw-rw-r--   0 michael   (1000) michael   (1000)       38 2023-07-08 06:30:08.921718 aiohttp-rpc-1.3.0b1/setup.cfg
+-rwxrwxrwx   0 michael   (1000) michael   (1000)     2287 2023-07-08 06:28:39.000000 aiohttp-rpc-1.3.0b1/setup.py
```

### Comparing `aiohttp-rpc-1.3.0/LICENSE.txt` & `aiohttp-rpc-1.3.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.3.0/PKG-INFO` & `aiohttp-rpc-1.3.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-rpc
-Version: 1.3.0
+Version: 1.3.0b1
 Summary: A simple JSON-RPC for aiohttp
 Home-page: https://github.com/expert-m/aiohttp-rpc/
 Author: Michael Sulyak
 Author-email: michael@sulyak.info
 License: MIT license
 Project-URL: GitHub: issues, https://github.com/expert-m/aiohttp-rpc/issues
 Project-URL: GitHub: repo, https://github.com/expert-m/aiohttp-rpc
@@ -31,15 +31,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # aiohttp-rpc
 
 [![PyPI](https://img.shields.io/pypi/v/aiohttp-rpc.svg?style=flat)](https://pypi.org/project/aiohttp-rpc/)
-[![PyPI - Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue?style=flat)](https://www.python.org/downloads/release/python-380/)
+[![PyPI - Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue?style=flat)](https://www.python.org/downloads/release/python-380/)
 [![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/expert-m/aiohttp-rpc.svg?style=flat)](https://scrutinizer-ci.com/g/expert-m/aiohttp-rpc/?branch=master)
 [![GitHub Issues](https://img.shields.io/github/issues/expert-m/aiohttp-rpc.svg?style=flat)](https://github.com/expert-m/aiohttp-rpc/issues)
 [![Gitter](https://img.shields.io/gitter/room/aiohttp-rpc/Lobby)](https://gitter.im/aiohttp-rpc/Lobby)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://opensource.org/licenses/MIT)
 
 > A library for a simple integration of the [JSON-RPC 2.0 protocol](https://www.jsonrpc.org/specification) to a Python application using [aiohttp](https://github.com/aio-libs/aiohttp).
 The motivation is to provide a simple, fast and reliable way to integrate the JSON-RPC 2.0 protocol into your application on the server and/or client side.
@@ -105,37 +105,37 @@
 ### HTTP Client Example
 ```python3
 import aiohttp_rpc
 import asyncio
 
 async def run():
     async with aiohttp_rpc.JsonRpcClient('http://0.0.0.0:8080/rpc') as rpc:
-        print('#1', await rpc.ping())
-        print('#2', await rpc.echo('one', 'two'))
-        print('#3', await rpc.call('echo', three='3'))
-        print('#4', await rpc.notify('echo', 123))
-        print('#5', await rpc.get_methods())
-        print('#6', await rpc.batch([
+        print('1', await rpc.ping())
+        print('4', await rpc.echo('one', 'two'))
+        print('3', await rpc.call('echo', three='3'))
+        print('5', await rpc.notify('echo', 123))
+        print('6', await rpc.get_methods())
+        print('7', await rpc.batch([
             ['echo', 2], 
             'echo2',
             'ping',
         ]))
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(run())
 ```
 
 This prints:
 ```text
-#1 pong
-#2 {'args': ['one', 'two'], 'kwargs': {}}
-#3 {'args': [], 'kwargs': {'three': '3'}}
-#4 None
-#5 {'get_method': {'doc': None, 'args': ['name'], 'kwargs': []}, 'get_methods': {'doc': None, 'args': [], 'kwargs': []}, 'ping': {'doc': None, 'args': ['rpc_request'], 'kwargs': []}, 'echo': {'doc': None, 'args': [], 'kwargs': []}}
-#6 ({'args': [2], 'kwargs': {}}, JsonRpcError(-32601, 'The method does not exist / is not available.'), 'pong')
+1 pong
+4 {'args': ['one', 'two'], 'kwargs': {}}
+3 {'args': [], 'kwargs': {'three': '3'}}
+5 None
+6 {'get_method': {'doc': None, 'args': ['name'], 'kwargs': []}, 'get_methods': {'doc': None, 'args': [], 'kwargs': []}, 'ping': {'doc': None, 'args': ['rpc_request'], 'kwargs': []}, 'echo': {'doc': None, 'args': [], 'kwargs': []}}
+7 ({'args': [2], 'kwargs': {}}, JsonRpcError(-32601, 'The method does not exist / is not available.'), 'pong')
 ```
 
 [back to top](#table-of-contents)
 
 ---
 
 <p align="center"><b>↑ This is enough to start :sunglasses: ↑</b></p>
```

### Comparing `aiohttp-rpc-1.3.0/README.md` & `aiohttp-rpc-1.3.0b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # aiohttp-rpc
 
 [![PyPI](https://img.shields.io/pypi/v/aiohttp-rpc.svg?style=flat)](https://pypi.org/project/aiohttp-rpc/)
-[![PyPI - Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue?style=flat)](https://www.python.org/downloads/release/python-380/)
+[![PyPI - Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue?style=flat)](https://www.python.org/downloads/release/python-380/)
 [![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/expert-m/aiohttp-rpc.svg?style=flat)](https://scrutinizer-ci.com/g/expert-m/aiohttp-rpc/?branch=master)
 [![GitHub Issues](https://img.shields.io/github/issues/expert-m/aiohttp-rpc.svg?style=flat)](https://github.com/expert-m/aiohttp-rpc/issues)
 [![Gitter](https://img.shields.io/gitter/room/aiohttp-rpc/Lobby)](https://gitter.im/aiohttp-rpc/Lobby)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://opensource.org/licenses/MIT)
 
 > A library for a simple integration of the [JSON-RPC 2.0 protocol](https://www.jsonrpc.org/specification) to a Python application using [aiohttp](https://github.com/aio-libs/aiohttp).
 The motivation is to provide a simple, fast and reliable way to integrate the JSON-RPC 2.0 protocol into your application on the server and/or client side.
@@ -71,37 +71,37 @@
 ### HTTP Client Example
 ```python3
 import aiohttp_rpc
 import asyncio
 
 async def run():
     async with aiohttp_rpc.JsonRpcClient('http://0.0.0.0:8080/rpc') as rpc:
-        print('#1', await rpc.ping())
-        print('#2', await rpc.echo('one', 'two'))
-        print('#3', await rpc.call('echo', three='3'))
-        print('#4', await rpc.notify('echo', 123))
-        print('#5', await rpc.get_methods())
-        print('#6', await rpc.batch([
+        print('1', await rpc.ping())
+        print('4', await rpc.echo('one', 'two'))
+        print('3', await rpc.call('echo', three='3'))
+        print('5', await rpc.notify('echo', 123))
+        print('6', await rpc.get_methods())
+        print('7', await rpc.batch([
             ['echo', 2], 
             'echo2',
             'ping',
         ]))
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(run())
 ```
 
 This prints:
 ```text
-#1 pong
-#2 {'args': ['one', 'two'], 'kwargs': {}}
-#3 {'args': [], 'kwargs': {'three': '3'}}
-#4 None
-#5 {'get_method': {'doc': None, 'args': ['name'], 'kwargs': []}, 'get_methods': {'doc': None, 'args': [], 'kwargs': []}, 'ping': {'doc': None, 'args': ['rpc_request'], 'kwargs': []}, 'echo': {'doc': None, 'args': [], 'kwargs': []}}
-#6 ({'args': [2], 'kwargs': {}}, JsonRpcError(-32601, 'The method does not exist / is not available.'), 'pong')
+1 pong
+4 {'args': ['one', 'two'], 'kwargs': {}}
+3 {'args': [], 'kwargs': {'three': '3'}}
+5 None
+6 {'get_method': {'doc': None, 'args': ['name'], 'kwargs': []}, 'get_methods': {'doc': None, 'args': [], 'kwargs': []}, 'ping': {'doc': None, 'args': ['rpc_request'], 'kwargs': []}, 'echo': {'doc': None, 'args': [], 'kwargs': []}}
+7 ({'args': [2], 'kwargs': {}}, JsonRpcError(-32601, 'The method does not exist / is not available.'), 'pong')
 ```
 
 [back to top](#table-of-contents)
 
 ---
 
 <p align="center"><b>↑ This is enough to start :sunglasses: ↑</b></p>
```

### Comparing `aiohttp-rpc-1.3.0/aiohttp_rpc/client/base.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/client/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
         return response
 
     async def direct_batch(self,
                            batch_request: protocol.JsonRpcBatchRequest,
                            **kwargs) -> typing.Optional[protocol.JsonRpcBatchResponse]:
         if not batch_request.requests:
-            raise errors.InvalidRequest('You can\'t send an empty batch request.')
+            raise errors.InvalidRequest('You can not send an empty batch request.')
 
         is_notification = batch_request.is_notification
 
         json_response, context = await self.send_json(
             batch_request.dump(),
             without_response=is_notification,
             **kwargs,
```

### Comparing `aiohttp-rpc-1.3.0/aiohttp_rpc/client/http.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/client/http.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.3.0/aiohttp_rpc/client/websocket.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/client/websocket.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,134 +16,104 @@
 logger = logging.getLogger(__name__)
 
 
 class WsJsonRpcClient(BaseJsonRpcClient):
     url: typing.Optional[str]
     ws_connect: typing.Optional[typedefs.WSConnectType]
     ws_connect_kwargs: dict
-    _timeout: typing.Optional[float]
-    _timeout_for_data_receiving: typing.Optional[float]
-    _connection_check_interval: typing.Optional[float]
+    timeout: typing.Optional[int]
     _pending: typing.Dict[typing.Any, asyncio.Future]
     _message_worker: typing.Optional[asyncio.Future] = None
-    _check_worker: typing.Optional[asyncio.Future] = None
     _session_is_outer: bool
     _ws_connect_is_outer: bool
     _json_request_handler: typing.Optional[typing.Callable] = None
     _unprocessed_json_response_handler: typing.Optional[typing.Callable] = None
     _background_tasks: typing.Set
-    _is_closed: bool = True
 
     def __init__(self,
                  url: typing.Optional[str] = None, *,
                  session: typing.Optional[ClientSession] = None,
                  ws_connect: typing.Optional[typedefs.WSConnectType] = None,
-                 timeout: typing.Optional[float] = 60,
-                 timeout_for_data_receiving: typing.Optional[float] = None,
-                 connection_check_interval: typing.Optional[float] = 5,
+                 timeout: typing.Optional[int] = 5,
                  json_request_handler: typing.Optional[typing.Callable] = None,
                  unprocessed_json_response_handler: typing.Optional[typing.Callable] = None,
                  **ws_connect_kwargs) -> None:
         assert (session is not None) or (url is not None and session is None) or (ws_connect is not None)
 
         self.url = url
-        self._timeout = timeout
-        self._timeout_for_data_receiving = timeout_for_data_receiving
-        self._connection_check_interval = connection_check_interval
+        self.timeout = timeout
 
         self.session = session
         self._session_is_outer = session is not None  # We don't close an outer session.
 
         self.ws_connect = ws_connect
         self.ws_connect_kwargs = ws_connect_kwargs
         self._ws_connect_is_outer = ws_connect is not None  # We don't close an outer WS connection.
 
         self._pending = {}
         self._json_request_handler = json_request_handler
         self._unprocessed_json_response_handler = unprocessed_json_response_handler
         self._background_tasks = set()
 
     async def connect(self) -> None:
-        self._is_closed = False
-
         if self.session is None and self.ws_connect is None:
             self.session = ClientSession(json_serialize=self.json_serialize)
 
         if self.ws_connect is None:
             assert self.url is not None and self.session is not None
 
             try:
                 self.ws_connect = await self.session.ws_connect(self.url, **self.ws_connect_kwargs)
             except Exception:
                 await self.disconnect()
                 raise
 
         self._message_worker = asyncio.create_task(self._handle_ws_messages())
 
-        if self._connection_check_interval is not None:
-            self._check_worker = asyncio.create_task(self._check_ws_connection())
-
     async def disconnect(self) -> None:
-        self._is_closed = True
-
         if self.ws_connect is not None and not self._ws_connect_is_outer:
             await self.ws_connect.close()
 
         if self.session is not None and not self._session_is_outer:
             await self.session.close()
 
         if self._message_worker is not None:
-            if self._ws_connect_is_outer:
-                await asyncio.wait_for(self._message_worker, timeout=60)
-            else:
-                await self._message_worker
-
-        if self._check_worker is not None:
-            self._check_worker.cancel()
-            await self._check_worker
+            await self._message_worker
 
     async def send_json(self,
                         data: typing.Any, *,
                         without_response: bool = False,
                         **kwargs) -> typing.Tuple[typing.Any, typing.Optional[dict]]:
         assert self.ws_connect is not None
 
         if without_response:
-            try:
-                await self.ws_connect.send_str(self.json_serialize(data), **kwargs)
-            except ConnectionResetError as e:
-                error = errors.ServerError(utils.get_exc_message(e)).with_traceback()
-                self._notify_all_about_error(error)
-                raise error
-
+            await self.ws_connect.send_str(self.json_serialize(data), **kwargs)
             return None, None
 
         request_ids = self._get_ids_from_json(data)
         future: asyncio.Future = asyncio.Future()
 
         for request_id in request_ids:
             self._pending[request_id] = future
 
-        try:
-            await self.ws_connect.send_str(self.json_serialize(data), **kwargs)
-        except ConnectionResetError as e:
-            error = errors.ServerError(utils.get_exc_message(e)).with_traceback()
-            self._notify_all_about_error(error)
-            raise error
+        await self.ws_connect.send_str(self.json_serialize(data), **kwargs)
 
         if not request_ids:
             return None, None
 
-        if self._timeout is not None:
-            future = asyncio.wait_for(future, timeout=self._timeout)  # type: ignore
+        if self.timeout is not None:
+            future = asyncio.wait_for(future, timeout=self.timeout)  # type: ignore
 
         result = await future
 
         return result, None
 
+    def clear_pending(self) -> None:
+        self._pending.clear()
+
     @staticmethod
     def _get_ids_from_json(data: typing.Any) -> typing.Tuple[typedefs.JsonRpcIdType, ...]:
         if not data:
             return ()
 
         if isinstance(data, typing.Mapping) and data.get('id') is not None:
             return (
@@ -158,73 +128,41 @@
             )
 
         return ()
 
     async def _handle_ws_messages(self) -> None:
         assert self.ws_connect is not None
 
-        while True:
-            try:
-                ws_msg: http_websocket.WSMessage = await self.ws_connect.receive(
-                    timeout=self._timeout_for_data_receiving,
-                )
-            except asyncio.TimeoutError:
-                if self._is_closed:
-                    break
-                else:
-                    continue
-
-            if ws_msg.type in (
-                    http_websocket.WSMsgType.CLOSE,
-                    http_websocket.WSMsgType.CLOSING,
-                    http_websocket.WSMsgType.CLOSED,
-            ):
-                break
+        ws_msg: http_websocket.WSMessage
 
+        async for ws_msg in self.ws_connect:
             if ws_msg.type != http_websocket.WSMsgType.TEXT:
                 continue
 
             try:
                 task = asyncio.create_task(self._handle_single_ws_message(ws_msg))
             except asyncio.CancelledError as e:
-                error = errors.InternalError(utils.get_exc_message(e)).with_traceback()
+                error = errors.ServerError(utils.get_exc_message(e)).with_traceback()
                 self._notify_all_about_error(error)
-                break
+                raise
             except Exception:
-                logger.warning('Can\'t process WS message.', exc_info=True)
+                logger.warning('Can not process WS message.', exc_info=True)
             else:
                 # To avoid a task disappearing mid execution:
                 self._background_tasks.add(task)
                 task.add_done_callback(self._background_tasks.discard)
 
-            if self._is_closed:
-                break
-
-    async def _check_ws_connection(self) -> None:
-        assert self.ws_connect is not None
-
-        try:
-            while not self._is_closed:
-                if self.ws_connect.closed:
-                    error = errors.ServerError('Connection is closed')
-                    self._notify_all_about_error(error)
-                    break
-
-                await asyncio.sleep(self._connection_check_interval)  # type: ignore
-        except asyncio.CancelledError:
-            pass
-
     async def _handle_single_ws_message(self, ws_msg: http_websocket.WSMessage) -> None:
         if ws_msg.type != http_websocket.WSMsgType.text:
             return
 
         try:
             json_response = json.loads(ws_msg.data)
         except Exception:
-            logger.warning('Can\'t parse json.', exc_info=True)
+            logger.warning('Cann\'t parse json.', exc_info=True)
             return
 
         if not json_response:
             return
 
         if isinstance(json_response, typing.Mapping):
             await self._handle_single_json_response(json_response, ws_msg=ws_msg)
@@ -267,22 +205,19 @@
             elif self._unprocessed_json_response_handler is not None:
                 self._unprocessed_json_response_handler(
                     ws_connect=self.ws_connect,
                     ws_msg=ws_msg,
                     json_response=json_responses,
                 )
 
-    def _notify_all_about_error(self, error: Exception) -> None:
+    def _notify_all_about_error(self, error: errors.JsonRpcError) -> None:
         for future in self._pending.values():
-            try:
-                future.set_exception(error)
-            except asyncio.InvalidStateError:
-                pass
+            future.set_exception(error)
 
-        self._pending.clear()
+        self.clear_pending()
 
     def _notify_about_result(self, response_id: typedefs.JsonRpcIdType, json_response: typing.Mapping) -> None:
         future = self._pending.pop(response_id, None)
 
         if future is not None:
             future.set_result(json_response)
 
@@ -292,11 +227,11 @@
         is_processed = False
 
         for response_id in response_ids:
             future = self._pending.pop(response_id, None)
 
             if future is not None and not is_processed:
                 # We suppose that a batch result has the same ids that we sent.
-                # And these ids have the same future.
+                # And this ids have the same future.
 
                 future.set_result(json_response)
                 is_processed = True
```

### Comparing `aiohttp-rpc-1.3.0/aiohttp_rpc/decorators.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/decorators.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.3.0/aiohttp_rpc/errors.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/errors.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.3.0/aiohttp_rpc/middlewares.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/middlewares.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.3.0/aiohttp_rpc/protocol/method.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/protocol/method.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.3.0/aiohttp_rpc/protocol/request.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/protocol/request.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.3.0/aiohttp_rpc/protocol/response.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/protocol/response.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.3.0/aiohttp_rpc/server/base.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/server/base.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.3.0/aiohttp_rpc/server/http.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/server/http.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.3.0/aiohttp_rpc/server/websocket.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/server/websocket.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.3.0/aiohttp_rpc/typedefs.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/typedefs.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.3.0/aiohttp_rpc/utils.py` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc/utils.py`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.3.0/aiohttp_rpc.egg-info/PKG-INFO` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-rpc
-Version: 1.3.0
+Version: 1.3.0b1
 Summary: A simple JSON-RPC for aiohttp
 Home-page: https://github.com/expert-m/aiohttp-rpc/
 Author: Michael Sulyak
 Author-email: michael@sulyak.info
 License: MIT license
 Project-URL: GitHub: issues, https://github.com/expert-m/aiohttp-rpc/issues
 Project-URL: GitHub: repo, https://github.com/expert-m/aiohttp-rpc
@@ -31,15 +31,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # aiohttp-rpc
 
 [![PyPI](https://img.shields.io/pypi/v/aiohttp-rpc.svg?style=flat)](https://pypi.org/project/aiohttp-rpc/)
-[![PyPI - Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue?style=flat)](https://www.python.org/downloads/release/python-380/)
+[![PyPI - Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue?style=flat)](https://www.python.org/downloads/release/python-380/)
 [![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/expert-m/aiohttp-rpc.svg?style=flat)](https://scrutinizer-ci.com/g/expert-m/aiohttp-rpc/?branch=master)
 [![GitHub Issues](https://img.shields.io/github/issues/expert-m/aiohttp-rpc.svg?style=flat)](https://github.com/expert-m/aiohttp-rpc/issues)
 [![Gitter](https://img.shields.io/gitter/room/aiohttp-rpc/Lobby)](https://gitter.im/aiohttp-rpc/Lobby)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://opensource.org/licenses/MIT)
 
 > A library for a simple integration of the [JSON-RPC 2.0 protocol](https://www.jsonrpc.org/specification) to a Python application using [aiohttp](https://github.com/aio-libs/aiohttp).
 The motivation is to provide a simple, fast and reliable way to integrate the JSON-RPC 2.0 protocol into your application on the server and/or client side.
@@ -105,37 +105,37 @@
 ### HTTP Client Example
 ```python3
 import aiohttp_rpc
 import asyncio
 
 async def run():
     async with aiohttp_rpc.JsonRpcClient('http://0.0.0.0:8080/rpc') as rpc:
-        print('#1', await rpc.ping())
-        print('#2', await rpc.echo('one', 'two'))
-        print('#3', await rpc.call('echo', three='3'))
-        print('#4', await rpc.notify('echo', 123))
-        print('#5', await rpc.get_methods())
-        print('#6', await rpc.batch([
+        print('1', await rpc.ping())
+        print('4', await rpc.echo('one', 'two'))
+        print('3', await rpc.call('echo', three='3'))
+        print('5', await rpc.notify('echo', 123))
+        print('6', await rpc.get_methods())
+        print('7', await rpc.batch([
             ['echo', 2], 
             'echo2',
             'ping',
         ]))
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(run())
 ```
 
 This prints:
 ```text
-#1 pong
-#2 {'args': ['one', 'two'], 'kwargs': {}}
-#3 {'args': [], 'kwargs': {'three': '3'}}
-#4 None
-#5 {'get_method': {'doc': None, 'args': ['name'], 'kwargs': []}, 'get_methods': {'doc': None, 'args': [], 'kwargs': []}, 'ping': {'doc': None, 'args': ['rpc_request'], 'kwargs': []}, 'echo': {'doc': None, 'args': [], 'kwargs': []}}
-#6 ({'args': [2], 'kwargs': {}}, JsonRpcError(-32601, 'The method does not exist / is not available.'), 'pong')
+1 pong
+4 {'args': ['one', 'two'], 'kwargs': {}}
+3 {'args': [], 'kwargs': {'three': '3'}}
+5 None
+6 {'get_method': {'doc': None, 'args': ['name'], 'kwargs': []}, 'get_methods': {'doc': None, 'args': [], 'kwargs': []}, 'ping': {'doc': None, 'args': ['rpc_request'], 'kwargs': []}, 'echo': {'doc': None, 'args': [], 'kwargs': []}}
+7 ({'args': [2], 'kwargs': {}}, JsonRpcError(-32601, 'The method does not exist / is not available.'), 'pong')
 ```
 
 [back to top](#table-of-contents)
 
 ---
 
 <p align="center"><b>↑ This is enough to start :sunglasses: ↑</b></p>
```

### Comparing `aiohttp-rpc-1.3.0/aiohttp_rpc.egg-info/SOURCES.txt` & `aiohttp-rpc-1.3.0b1/aiohttp_rpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiohttp-rpc-1.3.0/setup.py` & `aiohttp-rpc-1.3.0b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         long_description = file.read()
 
     packages = find_packages(exclude=['tests'])
     package_data = {package: ['py.typed'] for package in packages}
 
     setup(
         name='aiohttp-rpc',
-        version='1.3.0',
+        version='1.3.0b1',
         author='Michael Sulyak',
         url='https://github.com/expert-m/aiohttp-rpc/',
         author_email='michael@sulyak.info',
         keywords=[
             'aiohttp', 'asyncio', 'json-rpc', 'rpc',
         ],
         install_requires=[
```

