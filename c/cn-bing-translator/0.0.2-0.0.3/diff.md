# Comparing `tmp/cn_bing_translator-0.0.2.tar.gz` & `tmp/cn_bing_translator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cn_bing_translator-0.0.2.tar", last modified: Fri Jul 21 01:54:11 2023, max compression
+gzip compressed data, was "cn_bing_translator-0.0.3.tar", last modified: Fri Jul 21 06:12:37 2023, max compression
```

## Comparing `cn_bing_translator-0.0.2.tar` & `cn_bing_translator-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:54:11.937363 cn_bing_translator-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-21 01:54:02.000000 cn_bing_translator-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 01:54:02.000000 cn_bing_translator-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-21 01:54:11.937363 cn_bing_translator-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-21 01:54:02.000000 cn_bing_translator-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:54:11.937363 cn_bing_translator-0.0.2/cn_bing_translator/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-21 01:54:02.000000 cn_bing_translator-0.0.2/cn_bing_translator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-21 01:54:02.000000 cn_bing_translator-0.0.2/cn_bing_translator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-07-21 01:54:02.000000 cn_bing_translator-0.0.2/cn_bing_translator/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:54:11.937363 cn_bing_translator-0.0.2/cn_bing_translator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-21 01:54:11.000000 cn_bing_translator-0.0.2/cn_bing_translator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-21 01:54:11.000000 cn_bing_translator-0.0.2/cn_bing_translator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:54:11.000000 cn_bing_translator-0.0.2/cn_bing_translator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 01:54:11.000000 cn_bing_translator-0.0.2/cn_bing_translator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 01:54:11.000000 cn_bing_translator-0.0.2/cn_bing_translator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:54:11.937363 cn_bing_translator-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-21 01:54:02.000000 cn_bing_translator-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:12:37.155653 cn_bing_translator-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-21 06:12:19.000000 cn_bing_translator-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 06:12:19.000000 cn_bing_translator-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-21 06:12:37.155653 cn_bing_translator-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-21 06:12:19.000000 cn_bing_translator-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:12:37.155653 cn_bing_translator-0.0.3/cn_bing_translator/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-21 06:12:19.000000 cn_bing_translator-0.0.3/cn_bing_translator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-21 06:12:19.000000 cn_bing_translator-0.0.3/cn_bing_translator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-21 06:12:19.000000 cn_bing_translator-0.0.3/cn_bing_translator/requesttype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-07-21 06:12:19.000000 cn_bing_translator-0.0.3/cn_bing_translator/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:12:37.155653 cn_bing_translator-0.0.3/cn_bing_translator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-21 06:12:37.000000 cn_bing_translator-0.0.3/cn_bing_translator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-21 06:12:37.000000 cn_bing_translator-0.0.3/cn_bing_translator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 06:12:37.000000 cn_bing_translator-0.0.3/cn_bing_translator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 06:12:37.000000 cn_bing_translator-0.0.3/cn_bing_translator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 06:12:37.000000 cn_bing_translator-0.0.3/cn_bing_translator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 06:12:37.155653 cn_bing_translator-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-21 06:12:19.000000 cn_bing_translator-0.0.3/setup.py
```

### Comparing `cn_bing_translator-0.0.2/LICENSE` & `cn_bing_translator-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cn_bing_translator-0.0.2/PKG-INFO` & `cn_bing_translator-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,15 @@
-Metadata-Version: 2.1
-Name: cn_bing_translator
-Version: 0.0.2
-Summary: microsoft cn.bing translator
-Home-page: https://github.com/minibear2021/cn_bing_translator
-Author: minibear
-License: MIT
-Keywords: microsoft bing translator
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 微软bing翻译器python sdk
 
 [![PyPI version](https://badge.fury.io/py/cn_bing_translator.svg)](https://badge.fury.io/py/cn_bing_translator)
 [![Download count](https://img.shields.io/pypi/dm/cn_bing_translator)](https://img.shields.io/pypi/dm/cn_bing_translator)
 
 ## 介绍
 
-微软cn.bing翻译器，建议轻量使用，欢迎star、follow、fork：
+微软bing翻译器，支持cn.bing.com和www.bing.com，建议轻量使用，欢迎star、follow、fork。
 
 ## 适用对象
 
 无法或者不便使用微软Azaue Text Translation服务的用户轻量级用户可以使用bing提供的翻译能力。
 
 ## 源码
 
@@ -67,10 +54,18 @@
 如果有使用代理的需求，可以指定proxy：
 
 ```python
 proxy = {'https':'http://localhost:8080'}
 translator = Translator(proxy=proxy)
 ```
 
+默认调用cn.bing.com，如需使用www.bing.com，可以在初始化的时候指定：
+
+```python
+translator = Translator(cnBing=False)
+```
+
+需要注意的是，根据bing.com的跳转规则，如果服务器判断是中国区用户访问，即使指定cnBing为False，仍然会自动跳转到cn.bing.com。
+
 ## 注意事项
 
-建议轻量级使用，微软bing翻译器默认带有防滥用措施，短时间频繁发起大量请求可能会触发拦截。
+建议轻量级使用，控制调用量和频率，微软bing翻译器默认带有防滥用措施，频繁发起大量请求可能会触发拦截。
```

### Comparing `cn_bing_translator-0.0.2/README.md` & `cn_bing_translator-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,28 @@
+Metadata-Version: 2.1
+Name: cn_bing_translator
+Version: 0.0.3
+Summary: microsoft cn.bing translator
+Home-page: https://github.com/minibear2021/cn_bing_translator
+Author: minibear
+License: MIT
+Keywords: microsoft bing translator
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # 微软bing翻译器python sdk
 
 [![PyPI version](https://badge.fury.io/py/cn_bing_translator.svg)](https://badge.fury.io/py/cn_bing_translator)
 [![Download count](https://img.shields.io/pypi/dm/cn_bing_translator)](https://img.shields.io/pypi/dm/cn_bing_translator)
 
 ## 介绍
 
-微软cn.bing翻译器，建议轻量使用，欢迎star、follow、fork：
+微软bing翻译器，支持cn.bing.com和www.bing.com，建议轻量使用，欢迎star、follow、fork。
 
 ## 适用对象
 
 无法或者不便使用微软Azaue Text Translation服务的用户轻量级用户可以使用bing提供的翻译能力。
 
 ## 源码
 
@@ -54,10 +67,18 @@
 如果有使用代理的需求，可以指定proxy：
 
 ```python
 proxy = {'https':'http://localhost:8080'}
 translator = Translator(proxy=proxy)
 ```
 
+默认调用cn.bing.com，如需使用www.bing.com，可以在初始化的时候指定：
+
+```python
+translator = Translator(cnBing=False)
+```
+
+需要注意的是，根据bing.com的跳转规则，如果服务器判断是中国区用户访问，即使指定cnBing为False，仍然会自动跳转到cn.bing.com。
+
 ## 注意事项
 
-建议轻量级使用，微软bing翻译器默认带有防滥用措施，短时间频繁发起大量请求可能会触发拦截。
+建议轻量级使用，控制调用量和频率，微软bing翻译器默认带有防滥用措施，频繁发起大量请求可能会触发拦截。
```

### Comparing `cn_bing_translator-0.0.2/cn_bing_translator/exceptions.py` & `cn_bing_translator-0.0.3/cn_bing_translator/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,7 +14,11 @@
 
 class UnknownStatusCode(Exception):
     """Raised when http code is not 200"""
 
 
 class NoDataReceived(Exception):
     """Raised when no data is received from the server."""
+
+
+class UnknownRequestType(Exception):
+    """Raised when request type is unknown."""
```

### Comparing `cn_bing_translator-0.0.2/cn_bing_translator/translator.py` & `cn_bing_translator-0.0.3/cn_bing_translator/translator.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,50 +5,60 @@
 
 import json
 import re
 import time
 
 import requests
 
-from .exceptions import NoDataReceived, UnexpectedResponse, UnknownResponse, UnknownStatusCode
+from .exceptions import (UnexpectedResponse, UnknownRequestType,
+                         UnknownResponse, UnknownStatusCode)
+from .requesttype import RequestType
 
 
 class Translator:
-    def __init__(self, fromLang: str = "auto-detect", toLang: str = "en", agent: dict = {}, proxy: dict = {}, logger=None) -> None:
+    def __init__(self, fromLang: str = "auto-detect", toLang: str = "en", agent: dict = {}, proxy: dict = {}, logger=None, cnBing:bool = True) -> None:
         self._fromLang = fromLang
         self._toLang = toLang
         self._ig = self._iig = self._key = self._token = None
         self._timeout = 0
         self._session = requests.Session()
         self._session.proxies = proxy
         if not agent:
             agent = {'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.183 Safari/537.36'}
         self._session.headers.update(agent)
-        self._session.headers.update({'origin': 'https://cn.bing.com'})
-        self._session.headers.update({'referer': 'https://cn.bing.com/translator/'})
+        self._gateway = 'https://cn.bing.com' if cnBing else 'https://www.bing.com'
+        self._session.headers.update({'origin': f'{self._gateway}'})
+        self._session.headers.update({'referer': f'{self._gateway}/translator/'})
         self._url = ''
         self._logger = logger
-        # self._update_params()
 
-    def _update_params(self):
-        """
-        update params IG, IID, token, key
-        """
-        self._session.cookies.clear()
-        url = 'https://cn.bing.com/translator/'
-        response = self._session.get(url=url)
+    def _request(self, method: RequestType = RequestType.GET, url: str = '', data: dict = {}) -> requests.Response:
+        if method == RequestType.GET:
+            response = self._session.get(url=url)
+        elif method == RequestType.POST:
+            response = self._session.post(url=url, data=data)
+        else:
+            raise UnknownRequestType
         if self._logger:
-            self._logger.debug('Update params.')
             self._logger.debug(f'Request url: {url}')
-            self._logger.debug('Request type: get')
+            self._logger.debug(f'Request type: {method}')
             self._logger.debug(f'Request headers: {self._session.headers}')
+            self._logger.debug(f'Request data: {data}')
             self._logger.debug(f'Response status code: {response.status_code}')
             self._logger.debug(f'Response headers: {response.headers}')
             self._logger.debug(f'Response content: {response.text}')
+        return response
 
+    def _update_params(self) -> None:
+        """
+        update params IG, IID, token, key
+        """
+        self._session.cookies.clear()
+        url = f'{self._gateway}/translator/'
+        response = self._request(url=url)
         if response.status_code != 200:
             raise UnknownStatusCode
         iid = re.search(r'<div id="rich_tta" data-iid="(.*?)"', response.text)
         if iid:
             self._iid = iid.group(1)
         ig = re.search(',IG:"(.*?)",', response.text)
         if ig:
@@ -58,15 +68,15 @@
             self._key = match.group(1)
             self._token = match.group(2)
             self._timeout = int((time.time() - 600) * 1000) + int(match.group(3))
         if not (self._ig and self._iid and self._key and self._token and self._timeout):
             raise UnknownResponse
         if self._logger:
             self._logger.debug(f'iid: {self._iid}, ig: {self._ig}, key: {self._key}, token: {self._token}, timeout: {self._timeout}')
-        self._url = f'https://cn.bing.com/ttranslatev3?isVertical=1&IG={self._ig}&IID={self._iid}'
+        self._url = f'{self._gateway}/ttranslatev3?isVertical=1&IG={self._ig}&IID={self._iid}'
 
     def process(self, text: str, fromLang: str = '', toLang: str = '') -> str:
         """
         translate text from origin language
         """
         if self._timeout < int(time.time() * 1000):
             self._ig = self._iig = self._key = self._token = None
@@ -78,61 +88,42 @@
             'fromLang': fromLang if fromLang else self._fromLang,
             'text': f'{text}',
             'to': toLang if toLang else self._toLang,
             'token': self._token,
             'key': self._key,
             'tryFetchingGenderDebiasedTranslations': 'true'
         }
-        response = self._session.post(url=self._url, data=data)
-
-        if self._logger:
-            self._logger.debug(f'Request url: {self._url}')
-            self._logger.debug('Request type: post')
-            self._logger.debug(f'Request headers: {self._session.headers}')
-            self._logger.debug(f'Request data: {data}')
-            self._logger.debug(f'Response status code: {response.status_code}')
-            self._logger.debug(f'Response headers: {response.headers}')
-            self._logger.debug(f'Response content: {response.text}')
+        response = self._request(method=RequestType.POST, url=self._url, data=data)
         if response.status_code != 200:
             raise UnknownStatusCode
         try:
             content = json.loads(response.text)
         except:
             raise UnknownResponse
-        if type(content) == dict:  # and content.get('statusCode'):
-            # {"statusCode":205,"errorMessage":""}
-            print('status code error, update params')
+        if type(content) == dict:
             self._ig = self._iig = self._key = self._token = None
             self._timeout = 0
             self._update_params()
             data = {
                 '': '',
                 'fromLang': fromLang if fromLang else self._fromLang,
                 'text': f'{text}',
                 'to': toLang if toLang else self._toLang,
                 'token': self._token,
                 'key': self._key,
                 'tryFetchingGenderDebiasedTranslations': 'true'
             }
-            response = self._session.post(url=self._url, data=data)
-            if self._logger:
-                self._logger.debug(f'Request url: {self._url}')
-                self._logger.debug('Request type: post')
-                self._logger.debug(f'Request headers: {self._session.headers}')
-                self._logger.debug(f'Request data: {data}')
-                self._logger.debug(f'Response status code: {response.status_code}')
-                self._logger.debug(f'Response headers: {response.headers}')
-                self._logger.debug(f'Response content: {response.text}')
+            response = self._request(url=self._url, data=data)
             try:
                 content = json.loads(response.text)
             except:
                 raise UnknownResponse
             if response.status_code != 200:
                 raise UnknownStatusCode
-            if type(content) == dict:  # and content.get('statusCode'):
+            if type(content) == dict:
                 raise UnexpectedResponse
         result = ''
         try:
             if type(content) == list and type(content[0] == dict):
                 result = content[0].get('translations')[0].get('text')
             else:
                 raise UnknownResponse
```

### Comparing `cn_bing_translator-0.0.2/cn_bing_translator.egg-info/PKG-INFO` & `cn_bing_translator-0.0.3/cn_bing_translator.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cn-bing-translator
-Version: 0.0.2
+Version: 0.0.3
 Summary: microsoft cn.bing translator
 Home-page: https://github.com/minibear2021/cn_bing_translator
 Author: minibear
 License: MIT
 Keywords: microsoft bing translator
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 # 微软bing翻译器python sdk
 
 [![PyPI version](https://badge.fury.io/py/cn_bing_translator.svg)](https://badge.fury.io/py/cn_bing_translator)
 [![Download count](https://img.shields.io/pypi/dm/cn_bing_translator)](https://img.shields.io/pypi/dm/cn_bing_translator)
 
 ## 介绍
 
-微软cn.bing翻译器，建议轻量使用，欢迎star、follow、fork：
+微软bing翻译器，支持cn.bing.com和www.bing.com，建议轻量使用，欢迎star、follow、fork。
 
 ## 适用对象
 
 无法或者不便使用微软Azaue Text Translation服务的用户轻量级用户可以使用bing提供的翻译能力。
 
 ## 源码
 
@@ -67,10 +67,18 @@
 如果有使用代理的需求，可以指定proxy：
 
 ```python
 proxy = {'https':'http://localhost:8080'}
 translator = Translator(proxy=proxy)
 ```
 
+默认调用cn.bing.com，如需使用www.bing.com，可以在初始化的时候指定：
+
+```python
+translator = Translator(cnBing=False)
+```
+
+需要注意的是，根据bing.com的跳转规则，如果服务器判断是中国区用户访问，即使指定cnBing为False，仍然会自动跳转到cn.bing.com。
+
 ## 注意事项
 
-建议轻量级使用，微软bing翻译器默认带有防滥用措施，短时间频繁发起大量请求可能会触发拦截。
+建议轻量级使用，控制调用量和频率，微软bing翻译器默认带有防滥用措施，频繁发起大量请求可能会触发拦截。
```

### Comparing `cn_bing_translator-0.0.2/setup.py` & `cn_bing_translator-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf8") as f:
     long_description = f.read()
 
 setup(
     name="cn_bing_translator",
-    version="0.0.2",
+    version="0.0.3",
     author="minibear",
     description="microsoft cn.bing translator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     keywords="microsoft bing translator",
     url="https://github.com/minibear2021/cn_bing_translator",
```

