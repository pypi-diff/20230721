# Comparing `tmp/cn_bing_translator-0.0.1.tar.gz` & `tmp/cn_bing_translator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cn_bing_translator-0.0.1.tar", last modified: Thu Jul 20 08:03:04 2023, max compression
+gzip compressed data, was "cn_bing_translator-0.0.2.tar", last modified: Fri Jul 21 01:54:11 2023, max compression
```

## Comparing `cn_bing_translator-0.0.1.tar` & `cn_bing_translator-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-07-20 08:03:04.983636 cn_bing_translator-0.0.1/
--rw-r--r--   0 chen       (501) staff       (20)     1088 2022-09-27 05:53:26.000000 cn_bing_translator-0.0.1/LICENSE
--rw-r--r--   0 chen       (501) staff       (20)       17 2022-01-18 06:07:47.000000 cn_bing_translator-0.0.1/MANIFEST.in
--rw-r--r--   0 chen       (501) staff       (20)     2300 2023-07-20 08:03:04.983138 cn_bing_translator-0.0.1/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)     1910 2023-07-20 07:55:41.000000 cn_bing_translator-0.0.1/README.md
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-07-20 08:03:04.980739 cn_bing_translator-0.0.1/cn_bing_translator/
--rw-r--r--   0 chen       (501) staff       (20)       98 2023-07-20 05:56:15.000000 cn_bing_translator-0.0.1/cn_bing_translator/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)      561 2023-07-20 05:37:19.000000 cn_bing_translator-0.0.1/cn_bing_translator/exceptions.py
--rw-r--r--   0 chen       (501) staff       (20)     5604 2023-07-20 07:35:04.000000 cn_bing_translator-0.0.1/cn_bing_translator/translator.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-07-20 08:03:04.982521 cn_bing_translator-0.0.1/cn_bing_translator.egg-info/
--rw-r--r--   0 chen       (501) staff       (20)     2300 2023-07-20 08:03:04.000000 cn_bing_translator-0.0.1/cn_bing_translator.egg-info/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)      344 2023-07-20 08:03:04.000000 cn_bing_translator-0.0.1/cn_bing_translator.egg-info/SOURCES.txt
--rw-r--r--   0 chen       (501) staff       (20)        1 2023-07-20 08:03:04.000000 cn_bing_translator-0.0.1/cn_bing_translator.egg-info/dependency_links.txt
--rw-r--r--   0 chen       (501) staff       (20)       17 2023-07-20 08:03:04.000000 cn_bing_translator-0.0.1/cn_bing_translator.egg-info/requires.txt
--rw-r--r--   0 chen       (501) staff       (20)       19 2023-07-20 08:03:04.000000 cn_bing_translator-0.0.1/cn_bing_translator.egg-info/top_level.txt
--rw-r--r--   0 chen       (501) staff       (20)       38 2023-07-20 08:03:04.983755 cn_bing_translator-0.0.1/setup.cfg
--rw-r--r--   0 chen       (501) staff       (20)      662 2023-07-20 07:58:18.000000 cn_bing_translator-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:54:11.937363 cn_bing_translator-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-21 01:54:02.000000 cn_bing_translator-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 01:54:02.000000 cn_bing_translator-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-21 01:54:11.937363 cn_bing_translator-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-21 01:54:02.000000 cn_bing_translator-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:54:11.937363 cn_bing_translator-0.0.2/cn_bing_translator/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-21 01:54:02.000000 cn_bing_translator-0.0.2/cn_bing_translator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-21 01:54:02.000000 cn_bing_translator-0.0.2/cn_bing_translator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-07-21 01:54:02.000000 cn_bing_translator-0.0.2/cn_bing_translator/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:54:11.937363 cn_bing_translator-0.0.2/cn_bing_translator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-21 01:54:11.000000 cn_bing_translator-0.0.2/cn_bing_translator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-21 01:54:11.000000 cn_bing_translator-0.0.2/cn_bing_translator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:54:11.000000 cn_bing_translator-0.0.2/cn_bing_translator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 01:54:11.000000 cn_bing_translator-0.0.2/cn_bing_translator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 01:54:11.000000 cn_bing_translator-0.0.2/cn_bing_translator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:54:11.937363 cn_bing_translator-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-21 01:54:02.000000 cn_bing_translator-0.0.2/setup.py
```

### Comparing `cn_bing_translator-0.0.1/LICENSE` & `cn_bing_translator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cn_bing_translator-0.0.1/PKG-INFO` & `cn_bing_translator-0.0.2/cn_bing_translator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
-Name: cn_bing_translator
-Version: 0.0.1
+Name: cn-bing-translator
+Version: 0.0.2
 Summary: microsoft cn.bing translator
 Home-page: https://github.com/minibear2021/cn_bing_translator
 Author: minibear
 License: MIT
 Keywords: microsoft bing translator
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# 微信支付 API v3 Python SDK
+# 微软bing翻译器python sdk
 
 [![PyPI version](https://badge.fury.io/py/cn_bing_translator.svg)](https://badge.fury.io/py/cn_bing_translator)
 [![Download count](https://img.shields.io/pypi/dm/cn_bing_translator)](https://img.shields.io/pypi/dm/cn_bing_translator)
 
 ## 介绍
 
 微软cn.bing翻译器，建议轻量使用，欢迎star、follow、fork：
```

### Comparing `cn_bing_translator-0.0.1/README.md` & `cn_bing_translator-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 微信支付 API v3 Python SDK
+# 微软bing翻译器python sdk
 
 [![PyPI version](https://badge.fury.io/py/cn_bing_translator.svg)](https://badge.fury.io/py/cn_bing_translator)
 [![Download count](https://img.shields.io/pypi/dm/cn_bing_translator)](https://img.shields.io/pypi/dm/cn_bing_translator)
 
 ## 介绍
 
 微软cn.bing翻译器，建议轻量使用，欢迎star、follow、fork：
```

### Comparing `cn_bing_translator-0.0.1/cn_bing_translator/exceptions.py` & `cn_bing_translator-0.0.2/cn_bing_translator/exceptions.py`

 * *Files identical despite different names*

### Comparing `cn_bing_translator-0.0.1/cn_bing_translator/translator.py` & `cn_bing_translator-0.0.2/cn_bing_translator/translator.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,40 +12,34 @@
 from .exceptions import NoDataReceived, UnexpectedResponse, UnknownResponse, UnknownStatusCode
 
 
 class Translator:
     def __init__(self, fromLang: str = "auto-detect", toLang: str = "en", agent: dict = {}, proxy: dict = {}, logger=None) -> None:
         self._fromLang = fromLang
         self._toLang = toLang
-        self._ig = None
-        self._iid = None
-        self._key = None
-        self._token = None
-        self._timeout = None
+        self._ig = self._iig = self._key = self._token = None
+        self._timeout = 0
         self._session = requests.Session()
         self._session.proxies = proxy
         if not agent:
             agent = {'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.183 Safari/537.36'}
         self._session.headers.update(agent)
         self._session.headers.update({'origin': 'https://cn.bing.com'})
         self._session.headers.update({'referer': 'https://cn.bing.com/translator/'})
         self._url = ''
         self._logger = logger
-        self._update_params()
+        # self._update_params()
 
     def _update_params(self):
         """
         update params IG, IID, token, key
         """
+        self._session.cookies.clear()
         url = 'https://cn.bing.com/translator/'
         response = self._session.get(url=url)
-        # response = requests.get('https://cn.bing.com/translator/', headers=header)
-        # var params_AbusePreventionHelper = [1689738336956,"ccLhL60bQjpJ9MvZoTxZYlBRP_fNCUDi",3600000];
-        # IG:"BDEEA9DEA80F41D18B9EDDFD2A03985C",
-        # <div id="rich_tta" data-iid="translator.5026")">
         if self._logger:
             self._logger.debug('Update params.')
             self._logger.debug(f'Request url: {url}')
             self._logger.debug('Request type: get')
             self._logger.debug(f'Request headers: {self._session.headers}')
             self._logger.debug(f'Response status code: {response.status_code}')
             self._logger.debug(f'Response headers: {response.headers}')
@@ -62,32 +56,36 @@
         match = re.search(r'params_AbusePreventionHelper = \[(\d+),"(.*?)",(\d+)\];', response.text)
         if match:
             self._key = match.group(1)
             self._token = match.group(2)
             self._timeout = int((time.time() - 600) * 1000) + int(match.group(3))
         if not (self._ig and self._iid and self._key and self._token and self._timeout):
             raise UnknownResponse
+        if self._logger:
+            self._logger.debug(f'iid: {self._iid}, ig: {self._ig}, key: {self._key}, token: {self._token}, timeout: {self._timeout}')
         self._url = f'https://cn.bing.com/ttranslatev3?isVertical=1&IG={self._ig}&IID={self._iid}'
 
     def process(self, text: str, fromLang: str = '', toLang: str = '') -> str:
         """
         translate text from origin language
         """
+        if self._timeout < int(time.time() * 1000):
+            self._ig = self._iig = self._key = self._token = None
+            self._timeout = 0
+            self._update_params()
+
         data = {
             '': '',
             'fromLang': fromLang if fromLang else self._fromLang,
             'text': f'{text}',
             'to': toLang if toLang else self._toLang,
             'token': self._token,
             'key': self._key,
             'tryFetchingGenderDebiasedTranslations': 'true'
         }
-        if self._timeout < int(time.time()):
-            print('timeout, update params.')
-            self._update_params()
         response = self._session.post(url=self._url, data=data)
 
         if self._logger:
             self._logger.debug(f'Request url: {self._url}')
             self._logger.debug('Request type: post')
             self._logger.debug(f'Request headers: {self._session.headers}')
             self._logger.debug(f'Request data: {data}')
@@ -99,15 +97,26 @@
         try:
             content = json.loads(response.text)
         except:
             raise UnknownResponse
         if type(content) == dict:  # and content.get('statusCode'):
             # {"statusCode":205,"errorMessage":""}
             print('status code error, update params')
+            self._ig = self._iig = self._key = self._token = None
+            self._timeout = 0
             self._update_params()
+            data = {
+                '': '',
+                'fromLang': fromLang if fromLang else self._fromLang,
+                'text': f'{text}',
+                'to': toLang if toLang else self._toLang,
+                'token': self._token,
+                'key': self._key,
+                'tryFetchingGenderDebiasedTranslations': 'true'
+            }
             response = self._session.post(url=self._url, data=data)
             if self._logger:
                 self._logger.debug(f'Request url: {self._url}')
                 self._logger.debug('Request type: post')
                 self._logger.debug(f'Request headers: {self._session.headers}')
                 self._logger.debug(f'Request data: {data}')
                 self._logger.debug(f'Response status code: {response.status_code}')
```

### Comparing `cn_bing_translator-0.0.1/cn_bing_translator.egg-info/PKG-INFO` & `cn_bing_translator-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
-Name: cn-bing-translator
-Version: 0.0.1
+Name: cn_bing_translator
+Version: 0.0.2
 Summary: microsoft cn.bing translator
 Home-page: https://github.com/minibear2021/cn_bing_translator
 Author: minibear
 License: MIT
 Keywords: microsoft bing translator
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# 微信支付 API v3 Python SDK
+# 微软bing翻译器python sdk
 
 [![PyPI version](https://badge.fury.io/py/cn_bing_translator.svg)](https://badge.fury.io/py/cn_bing_translator)
 [![Download count](https://img.shields.io/pypi/dm/cn_bing_translator)](https://img.shields.io/pypi/dm/cn_bing_translator)
 
 ## 介绍
 
 微软cn.bing翻译器，建议轻量使用，欢迎star、follow、fork：
```

### Comparing `cn_bing_translator-0.0.1/setup.py` & `cn_bing_translator-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf8") as f:
     long_description = f.read()
 
 setup(
     name="cn_bing_translator",
-    version="0.0.1",
+    version="0.0.2",
     author="minibear",
     description="microsoft cn.bing translator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     keywords="microsoft bing translator",
     url="https://github.com/minibear2021/cn_bing_translator",
```

