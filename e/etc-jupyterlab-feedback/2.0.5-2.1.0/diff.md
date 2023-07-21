# Comparing `tmp/etc_jupyterlab_feedback-2.0.5.tar.gz` & `tmp/etc_jupyterlab_feedback-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etc_jupyterlab_feedback-2.0.5.tar", last modified: Tue Sep  6 12:43:26 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `etc_jupyterlab_feedback-2.0.5.tar` & `etc_jupyterlab_feedback-2.1.0.tar`

### file list

```diff
@@ -1,60 +1,43 @@
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-09-06 12:43:26.861184 etc_jupyterlab_feedback-2.0.5/
--rw-rw-r--   0 null      (1000) null      (1000)       86 2022-08-22 13:11:10.000000 etc_jupyterlab_feedback-2.0.5/CHANGELOG.md
--rw-rw-r--   0 null      (1000) null      (1000)     1511 2022-08-22 13:11:10.000000 etc_jupyterlab_feedback-2.0.5/LICENSE
--rw-rw-r--   0 null      (1000) null      (1000)      470 2022-08-22 13:11:10.000000 etc_jupyterlab_feedback-2.0.5/MANIFEST.in
--rw-rw-r--   0 null      (1000) null      (1000)     4390 2022-09-06 12:43:26.861184 etc_jupyterlab_feedback-2.0.5/PKG-INFO
--rw-rw-r--   0 null      (1000) null      (1000)     3343 2022-08-25 20:41:53.000000 etc_jupyterlab_feedback-2.0.5/README.md
--rw-rw-r--   0 null      (1000) null      (1000)     1905 2022-08-22 13:11:10.000000 etc_jupyterlab_feedback-2.0.5/RELEASE.md
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-09-06 12:43:26.856184 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/
--rw-rw-r--   0 null      (1000) null      (1000)      602 2022-08-22 18:37:47.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/__init__.py
--rw-rw-r--   0 null      (1000) null      (1000)      625 2022-08-22 13:11:10.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/_version.py
--rw-rw-r--   0 null      (1000) null      (1000)     1060 2022-08-25 22:12:58.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/application.py
--rw-rw-r--   0 null      (1000) null      (1000)     4206 2022-08-25 22:21:31.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/handlers.py
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-09-06 12:43:26.858183 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/labextension/
--rw-rw-r--   0 null      (1000) null      (1000)    21710 2022-09-06 12:43:05.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/labextension/build_log.json
--rw-rw-r--   0 null      (1000) null      (1000)     4051 2022-09-06 12:43:06.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/labextension/package.json
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-09-06 12:43:26.851184 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/labextension/schemas/
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-09-06 12:43:26.851184 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/labextension/schemas/@educational-technology-collective/
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-09-06 12:43:26.858183 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/labextension/schemas/@educational-technology-collective/etc_jupyterlab_feedback/
--rw-rw-r--   0 null      (1000) null      (1000)     3909 2022-09-06 12:43:05.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/labextension/schemas/@educational-technology-collective/etc_jupyterlab_feedback/package.json.orig
--rw-rw-r--   0 null      (1000) null      (1000)      269 2022-09-06 12:43:05.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/labextension/schemas/@educational-technology-collective/etc_jupyterlab_feedback/plugin.json
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-09-06 12:43:26.860184 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/labextension/static/
--rw-rw-r--   0 null      (1000) null      (1000)    17090 2022-09-06 12:43:06.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/labextension/static/lib_index_js.706e3844fb1e47ea9e82.js
--rw-rw-r--   0 null      (1000) null      (1000)    14162 2022-09-06 12:43:06.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/labextension/static/lib_index_js.706e3844fb1e47ea9e82.js.map
--rw-rw-r--   0 null      (1000) null      (1000)    29477 2022-09-06 12:43:06.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/labextension/static/remoteEntry.8711752c2aaf5ce12063.js
--rw-rw-r--   0 null      (1000) null      (1000)    28934 2022-09-06 12:43:06.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/labextension/static/remoteEntry.8711752c2aaf5ce12063.js.map
--rw-rw-r--   0 null      (1000) null      (1000)      201 2022-09-06 12:43:05.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/labextension/static/style.js
--rw-rw-r--   0 null      (1000) null      (1000)     4911 2022-09-06 12:43:06.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/labextension/static/style_index_js.ab85a44818daaf520017.js
--rw-rw-r--   0 null      (1000) null      (1000)     2240 2022-09-06 12:43:06.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/labextension/static/style_index_js.ab85a44818daaf520017.js.map
--rw-rw-r--   0 null      (1000) null      (1000)    12146 2022-09-06 12:43:06.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f401fe20d789473d9301.js
--rw-rw-r--   0 null      (1000) null      (1000)    13922 2022-09-06 12:43:06.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f401fe20d789473d9301.js.map
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-09-06 12:43:26.857184 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback.egg-info/
--rw-rw-r--   0 null      (1000) null      (1000)     4390 2022-09-06 12:43:26.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback.egg-info/PKG-INFO
--rw-rw-r--   0 null      (1000) null      (1000)     2023 2022-09-06 12:43:26.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback.egg-info/SOURCES.txt
--rw-rw-r--   0 null      (1000) null      (1000)        1 2022-09-06 12:43:26.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback.egg-info/dependency_links.txt
--rw-rw-r--   0 null      (1000) null      (1000)        1 2022-08-22 13:12:49.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback.egg-info/not-zip-safe
--rw-rw-r--   0 null      (1000) null      (1000)       31 2022-09-06 12:43:26.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback.egg-info/requires.txt
--rw-rw-r--   0 null      (1000) null      (1000)       24 2022-09-06 12:43:26.000000 etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback.egg-info/top_level.txt
--rw-rw-r--   0 null      (1000) null      (1000)      207 2022-08-22 13:11:10.000000 etc_jupyterlab_feedback-2.0.5/install.json
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-09-06 12:43:26.851184 etc_jupyterlab_feedback-2.0.5/jupyter-config/
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-09-06 12:43:26.860184 etc_jupyterlab_feedback-2.0.5/jupyter-config/nb-config/
--rw-rw-r--   0 null      (1000) null      (1000)      100 2022-08-22 13:11:10.000000 etc_jupyterlab_feedback-2.0.5/jupyter-config/nb-config/etc_jupyterlab_feedback.json
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-09-06 12:43:26.860184 etc_jupyterlab_feedback-2.0.5/jupyter-config/server-config/
--rw-rw-r--   0 null      (1000) null      (1000)       98 2022-08-22 13:11:10.000000 etc_jupyterlab_feedback-2.0.5/jupyter-config/server-config/etc_jupyterlab_feedback.json
--rw-rw-r--   0 null      (1000) null      (1000)     3909 2022-09-06 12:42:59.000000 etc_jupyterlab_feedback-2.0.5/package.json
--rw-rw-r--   0 null      (1000) null      (1000)      627 2022-08-22 13:11:10.000000 etc_jupyterlab_feedback-2.0.5/pyproject.toml
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-09-06 12:43:26.860184 etc_jupyterlab_feedback-2.0.5/schema/
--rw-rw-r--   0 null      (1000) null      (1000)      269 2022-08-22 13:11:10.000000 etc_jupyterlab_feedback-2.0.5/schema/plugin.json
--rw-rw-r--   0 null      (1000) null      (1000)       38 2022-09-06 12:43:26.861184 etc_jupyterlab_feedback-2.0.5/setup.cfg
--rw-rw-r--   0 null      (1000) null      (1000)     3282 2022-08-22 13:11:10.000000 etc_jupyterlab_feedback-2.0.5/setup.py
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-09-06 12:43:26.861184 etc_jupyterlab_feedback-2.0.5/src/
--rw-rw-r--   0 null      (1000) null      (1000)     2236 2022-08-23 20:50:22.000000 etc_jupyterlab_feedback-2.0.5/src/button.ts
--rw-rw-r--   0 null      (1000) null      (1000)     1110 2022-08-22 13:11:10.000000 etc_jupyterlab_feedback-2.0.5/src/handler.ts
--rw-rw-r--   0 null      (1000) null      (1000)     2816 2022-08-24 15:46:25.000000 etc_jupyterlab_feedback-2.0.5/src/index.ts
--rw-rw-r--   0 null      (1000) null      (1000)     7423 2022-09-06 12:41:57.000000 etc_jupyterlab_feedback-2.0.5/src/service.ts
-drwxrwxr-x   0 null      (1000) null      (1000)        0 2022-09-06 12:43:26.861184 etc_jupyterlab_feedback-2.0.5/style/
--rw-rw-r--   0 null      (1000) null      (1000)      221 2022-08-23 13:38:28.000000 etc_jupyterlab_feedback-2.0.5/style/base.css
--rw-rw-r--   0 null      (1000) null      (1000)       25 2022-08-22 13:11:10.000000 etc_jupyterlab_feedback-2.0.5/style/index.css
--rw-rw-r--   0 null      (1000) null      (1000)       21 2022-08-22 13:11:10.000000 etc_jupyterlab_feedback-2.0.5/style/index.js
--rw-rw-r--   0 null      (1000) null      (1000)      555 2022-08-22 13:23:24.000000 etc_jupyterlab_feedback-2.0.5/tsconfig.json
--rw-rw-r--   0 null      (1000) null      (1000)   295344 2022-08-22 13:26:29.000000 etc_jupyterlab_feedback-2.0.5/yarn.lock
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/.copier-answers.yml
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/.eslintrc.js
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/.stylelintrc
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/RELEASE.md
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/install.json
+-rw-r--r--   0        0        0   704564 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/package-lock.json
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/tsconfig.json
+-rw-r--r--   0        0        0   218367 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/yarn.lock
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/etc_jupyterlab_feedback/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/etc_jupyterlab_feedback/_version.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/etc_jupyterlab_feedback/application.py
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/etc_jupyterlab_feedback/handlers.py
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/etc_jupyterlab_feedback/labextension/package.json
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/etc_jupyterlab_feedback/labextension/schemas/@educational-technology-collective/etc_jupyterlab_feedback/package.json.orig
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/etc_jupyterlab_feedback/labextension/schemas/@educational-technology-collective/etc_jupyterlab_feedback/plugin.json
+-rw-r--r--   0        0        0     5239 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/etc_jupyterlab_feedback/labextension/static/261.577b1631aa92edfe911e.js
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/etc_jupyterlab_feedback/labextension/static/747.7ff222fe27eb90d3fdad.js
+-rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/etc_jupyterlab_feedback/labextension/static/remoteEntry.8f6feffc7063e14f2def.js
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/etc_jupyterlab_feedback/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/etc_jupyterlab_feedback/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/jupyter-config/nb-config/etc_jupyterlab_feedback.json
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/jupyter-config/server-config/etc_jupyterlab_feedback.json
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/schema/plugin.json
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/src/button.ts
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/src/handler.ts
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/src/index.ts
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/src/service.ts
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/stack/Untitled.json
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/style/index.js
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/LICENSE
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/README.md
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 etc_jupyterlab_feedback-2.1.0/PKG-INFO
```

### Comparing `etc_jupyterlab_feedback-2.0.5/LICENSE` & `etc_jupyterlab_feedback-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/__init__.py` & `etc_jupyterlab_feedback-2.1.0/etc_jupyterlab_feedback/__init__.py`

 * *Files identical despite different names*

### Comparing `etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/application.py` & `etc_jupyterlab_feedback-2.1.0/etc_jupyterlab_feedback/application.py`

 * *Files identical despite different names*

### Comparing `etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/handlers.py` & `etc_jupyterlab_feedback-2.1.0/etc_jupyterlab_feedback/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import json
 import traceback
-from ._version import _fetchVersion
+from ._version import VERSION
 from requests import Session, Request
 from jupyter_server.base.handlers import JupyterHandler
 from jupyter_server.extension.handler import ExtensionHandlerMixin
 import tornado
 import urllib.request
 from os.path import join, expanduser
 import subprocess
 from tornado.ioloop import IOLoop
 import uuid
+import time
 
 MACHINE_ID = str(uuid.uuid4())
 
 class HTTPException(Exception):
     def __init__(self, code, message):
         self.code = code
         self.message = message
@@ -23,15 +24,15 @@
     def get(self, resource):
         try:
             self.set_header('content-type', 'application/json')
             if resource == 'config':
                 self.finish(json.dumps({
                     'nbgrader_validate_enabled': self.extensionapp.nbgrader_validate_enabled,
                     'feedback_enabled': self.extensionapp.feedback_enabled,
-                    'version':  _fetchVersion()
+                    'version':  VERSION
                 }))
             else:
                 self.set_status(404)
 
         except Exception as e:
             self.set_status(500)
             self.log.error(traceback.format_exc())
@@ -61,53 +62,53 @@
             self.set_status(500)
             self.log.error(traceback.format_exc())
 
     def feedback(self, data):
 
         fullpath = expanduser(
             join(self.settings['server_root_dir'], data['notebook_path']))
-
+        
         with open(fullpath, 'rb') as f:
             data = json.load(f)
 
-            for cell in data['cells']:
-                if 'outputs' in cell:
-                    cell['outputs'] = []
-
-            data['metadata']['etc_machine_id'] = MACHINE_ID
-
-            data = json.dumps(data).encode('utf-8')
-
-            with Session() as s:
-
-                req = Request(
-                    'POST',
-                    self.extensionapp.feedback_url,
-                    data=data,
-                    headers={
-                        'accept': 'application/json',
-                        'content-type': 'application/json'
-                    })
-
-                prepped = s.prepare_request(req)
-
-                if self.extensionapp.cert_path:
-                    res = s.send(
-                        prepped, 
-                        proxies=urllib.request.getproxies(),
-                        timeout=self.extensionapp.feedback_timeout,
-                        verify=self.extensionapp.cert_path)
-                else:
-                    res = s.send(
-                        prepped, 
-                        proxies=urllib.request.getproxies(),
-                        timeout=self.extensionapp.feedback_timeout
-                        )
+        for cell in data['cells']:
+            if 'outputs' in cell:
+                cell['outputs'] = []
+
+        data['metadata']['etc_machine_id'] = MACHINE_ID
+
+        data = json.dumps(data).encode('utf-8')
+        
+        with Session() as s:
+
+            req = Request(
+                'POST',
+                self.extensionapp.feedback_url,
+                data=data,
+                headers={
+                    'accept': 'application/json',
+                    'content-type': 'application/json'
+                })
+
+            prepped = s.prepare_request(req)
+
+            if self.extensionapp.cert_path:
+                res = s.send(
+                    prepped, 
+                    proxies=urllib.request.getproxies(),
+                    timeout=self.extensionapp.feedback_timeout,
+                    verify=self.extensionapp.cert_path)
+            else:
+                res = s.send(
+                    prepped, 
+                    proxies=urllib.request.getproxies(),
+                    timeout=self.extensionapp.feedback_timeout
+                    )
 
-                return res.content.decode('utf-8')
+            return res.content.decode('utf-8')
 
     def nbgrader_validate(self, data):
         
         fullpath = expanduser(
             join(self.settings['server_root_dir'], data['notebook_path']))
         full_output = subprocess.run(
             ["nbgrader", "validate", fullpath],
```

### Comparing `etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/labextension/package.json` & `etc_jupyterlab_feedback-2.1.0/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9400432900432901%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.2', '@jupyterlab/coreutils': '^6.0.2', "*

 * *                   "'@jupyterlab/notebook': '^4.0.2', '@jupyterlab/services': '^7.0.2', "*

 * *                   "'@jupyterlab/settingregistry': '^4.0.2'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', '@typescript-eslint/eslint-plugin': "*

 * *                      "'^5.55.0', '@typescript-eslint/parser': '^5.55.0', 'eslint': '^8.36.0', "*

 * *                      "'eslint-config-prettier': '^8.8.0', 'eslint-plugi […]*

```diff
@@ -3,62 +3,64 @@
         "email": "",
         "name": "ETC"
     },
     "bugs": {
         "url": "https://github.com/educational-technology-collective/etc_jupyterlab_feedback/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.1.0",
-        "@jupyterlab/coreutils": "^5.1.0",
-        "@jupyterlab/notebook": "^3.0.7",
-        "@jupyterlab/services": "^6.1.0",
-        "@jupyterlab/settingregistry": "^3.1.0"
+        "@jupyterlab/application": "^4.0.2",
+        "@jupyterlab/coreutils": "^6.0.2",
+        "@jupyterlab/notebook": "^4.0.2",
+        "@jupyterlab/services": "^7.0.2",
+        "@jupyterlab/settingregistry": "^4.0.2"
     },
     "description": "A JupyterLab extension.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.1.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.15.0",
-        "eslint-plugin-prettier": "^3.1.4",
+        "@jupyterlab/builder": "^4.0.0",
+        "@types/json-schema": "^7.0.11",
+        "@types/react": "^18.0.26",
+        "@typescript-eslint/eslint-plugin": "^5.55.0",
+        "@typescript-eslint/parser": "^5.55.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.8.0",
+        "eslint-plugin-prettier": "^5.0.0",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "stylelint": "^14.3.0",
+        "prettier": "^3.0.0",
+        "rimraf": "^4.4.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^15.10.1",
         "stylelint-config-prettier": "^9.0.3",
-        "stylelint-config-recommended": "^6.0.0",
-        "stylelint-config-standard": "~24.0.0",
-        "stylelint-prettier": "^2.0.0",
-        "typescript": "~4.1.3"
+        "stylelint-config-recommended": "^13.0.0",
+        "stylelint-config-standard": "^34.0.0",
+        "stylelint-prettier": "^4.0.0",
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.40"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
-        "schema/*.json"
+        "schema/*.json",
+        "style/index.js"
     ],
     "homepage": "https://github.com/educational-technology-collective/etc_jupyterlab_feedback",
     "jupyter-releaser": {
         "hooks": {
             "before-build-npm": [
                 "python -m pip install jupyterlab~=3.1",
                 "jlpm"
             ],
             "before-build-python": [
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.8711752c2aaf5ce12063.js",
-            "style": "./style"
-        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "etc_jupyterlab_feedback"
                 },
                 "managers": [
                     "pip"
@@ -113,9 +115,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.0.5"
+    "version": "2.1.0"
 }
```

### Comparing `etc_jupyterlab_feedback-2.0.5/etc_jupyterlab_feedback/labextension/schemas/@educational-technology-collective/etc_jupyterlab_feedback/package.json.orig` & `etc_jupyterlab_feedback-2.1.0/etc_jupyterlab_feedback/labextension/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9400432900432901%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.2', '@jupyterlab/coreutils': '^6.0.2', "*

 * *                   "'@jupyterlab/notebook': '^4.0.2', '@jupyterlab/services': '^7.0.2', "*

 * *                   "'@jupyterlab/settingregistry': '^4.0.2'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', '@typescript-eslint/eslint-plugin': "*

 * *                      "'^5.55.0', '@typescript-eslint/parser': '^5.55.0', 'eslint': '^8.36.0', "*

 * *                      "'eslint-config-prettier': '^8.8.0', 'eslint-plugi […]*

```diff
@@ -3,57 +3,69 @@
         "email": "",
         "name": "ETC"
     },
     "bugs": {
         "url": "https://github.com/educational-technology-collective/etc_jupyterlab_feedback/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.1.0",
-        "@jupyterlab/coreutils": "^5.1.0",
-        "@jupyterlab/notebook": "^3.0.7",
-        "@jupyterlab/services": "^6.1.0",
-        "@jupyterlab/settingregistry": "^3.1.0"
+        "@jupyterlab/application": "^4.0.2",
+        "@jupyterlab/coreutils": "^6.0.2",
+        "@jupyterlab/notebook": "^4.0.2",
+        "@jupyterlab/services": "^7.0.2",
+        "@jupyterlab/settingregistry": "^4.0.2"
     },
     "description": "A JupyterLab extension.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.1.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.15.0",
-        "eslint-plugin-prettier": "^3.1.4",
+        "@jupyterlab/builder": "^4.0.0",
+        "@types/json-schema": "^7.0.11",
+        "@types/react": "^18.0.26",
+        "@typescript-eslint/eslint-plugin": "^5.55.0",
+        "@typescript-eslint/parser": "^5.55.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.8.0",
+        "eslint-plugin-prettier": "^5.0.0",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "stylelint": "^14.3.0",
+        "prettier": "^3.0.0",
+        "rimraf": "^4.4.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^15.10.1",
         "stylelint-config-prettier": "^9.0.3",
-        "stylelint-config-recommended": "^6.0.0",
-        "stylelint-config-standard": "~24.0.0",
-        "stylelint-prettier": "^2.0.0",
-        "typescript": "~4.1.3"
+        "stylelint-config-recommended": "^13.0.0",
+        "stylelint-config-standard": "^34.0.0",
+        "stylelint-prettier": "^4.0.0",
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.40"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
-        "schema/*.json"
+        "schema/*.json",
+        "style/index.js"
     ],
     "homepage": "https://github.com/educational-technology-collective/etc_jupyterlab_feedback",
     "jupyter-releaser": {
         "hooks": {
             "before-build-npm": [
                 "python -m pip install jupyterlab~=3.1",
                 "jlpm"
             ],
             "before-build-python": [
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.8f6feffc7063e14f2def.js",
+            "style": "./style"
+        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "etc_jupyterlab_feedback"
                 },
                 "managers": [
                     "pip"
@@ -108,9 +120,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.0.5"
+    "version": "2.1.0"
 }
```

### Comparing `etc_jupyterlab_feedback-2.0.5/package.json` & `etc_jupyterlab_feedback-2.1.0/etc_jupyterlab_feedback/labextension/schemas/@educational-technology-collective/etc_jupyterlab_feedback/package.json.orig`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.944805194805195%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.2', '@jupyterlab/coreutils': '^6.0.2', "*

 * *                   "'@jupyterlab/notebook': '^4.0.2', '@jupyterlab/services': '^7.0.2', "*

 * *                   "'@jupyterlab/settingregistry': '^4.0.2'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', '@typescript-eslint/eslint-plugin': "*

 * *                      "'^5.55.0', '@typescript-eslint/parser': '^5.55.0', 'eslint': '^8.36.0', "*

 * *                      "'eslint-config-prettier': '^8.8.0', 'eslint-plugi […]*

```diff
@@ -3,43 +3,50 @@
         "email": "",
         "name": "ETC"
     },
     "bugs": {
         "url": "https://github.com/educational-technology-collective/etc_jupyterlab_feedback/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.1.0",
-        "@jupyterlab/coreutils": "^5.1.0",
-        "@jupyterlab/notebook": "^3.0.7",
-        "@jupyterlab/services": "^6.1.0",
-        "@jupyterlab/settingregistry": "^3.1.0"
+        "@jupyterlab/application": "^4.0.2",
+        "@jupyterlab/coreutils": "^6.0.2",
+        "@jupyterlab/notebook": "^4.0.2",
+        "@jupyterlab/services": "^7.0.2",
+        "@jupyterlab/settingregistry": "^4.0.2"
     },
     "description": "A JupyterLab extension.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.1.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.15.0",
-        "eslint-plugin-prettier": "^3.1.4",
+        "@jupyterlab/builder": "^4.0.0",
+        "@types/json-schema": "^7.0.11",
+        "@types/react": "^18.0.26",
+        "@typescript-eslint/eslint-plugin": "^5.55.0",
+        "@typescript-eslint/parser": "^5.55.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.8.0",
+        "eslint-plugin-prettier": "^5.0.0",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "stylelint": "^14.3.0",
+        "prettier": "^3.0.0",
+        "rimraf": "^4.4.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^15.10.1",
         "stylelint-config-prettier": "^9.0.3",
-        "stylelint-config-recommended": "^6.0.0",
-        "stylelint-config-standard": "~24.0.0",
-        "stylelint-prettier": "^2.0.0",
-        "typescript": "~4.1.3"
+        "stylelint-config-recommended": "^13.0.0",
+        "stylelint-config-standard": "^34.0.0",
+        "stylelint-prettier": "^4.0.0",
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.40"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
-        "schema/*.json"
+        "schema/*.json",
+        "style/index.js"
     ],
     "homepage": "https://github.com/educational-technology-collective/etc_jupyterlab_feedback",
     "jupyter-releaser": {
         "hooks": {
             "before-build-npm": [
                 "python -m pip install jupyterlab~=3.1",
                 "jlpm"
@@ -108,9 +115,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.0.5"
+    "version": "2.1.0"
 }
```

### Comparing `etc_jupyterlab_feedback-2.0.5/src/button.ts` & `etc_jupyterlab_feedback-2.1.0/src/button.ts`

 * *Files identical despite different names*

### Comparing `etc_jupyterlab_feedback-2.0.5/src/handler.ts` & `etc_jupyterlab_feedback-2.1.0/src/handler.ts`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     'etc-jupyterlab-feedback', // API Namespace
     endPoint
   );
 
   let response: Response;
   try {
     response = await ServerConnection.makeRequest(requestUrl, init, settings);
-  } catch (error) {
+  } catch (error: any) {
     throw new ServerConnection.NetworkError(error);
   }
 
   let data: any = await response.text();
 
   if (data.length > 0) {
     try {
```

### Comparing `etc_jupyterlab_feedback-2.0.5/src/index.ts` & `etc_jupyterlab_feedback-2.1.0/src/index.ts`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-import { each } from '@lumino/algorithm';
-
-import { ISignal, Signal } from "@lumino/signaling";
-
 import { Token } from '@lumino/coreutils';
 
 import {
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 
@@ -62,35 +58,14 @@
       try {
 
         await app.started;
 
         const config = await requestAPI<any>('config');
 
         console.log(`${PLUGIN_ID}, ${config.version}`);
-
-        // //// TEST
-        // function addButtonToToolbar(notebookPanel: NotebookPanel) {
-
-        //   let etcJupyterLabFeedbackService = etcJupyterLabFeedbackServiceFactory.create({ notebookPanel });
-
-        //   etcJupyterLabFeedbackService.buttonClicked.connect((sender, args) => console.log(args));
-        //   etcJupyterLabFeedbackService.resultsDisplayed.connect((sender, args) => console.log(args));
-        //   etcJupyterLabFeedbackService.resultsDismissed.connect((sender, args) => console.log(args));
-        // }
-
-        // notebookTracker.forEach(addButtonToToolbar);
-
-        // notebookTracker.widgetAdded.connect(async (sender: INotebookTracker, notebookPanel: NotebookPanel) => {
-
-        //   await notebookPanel.revealed;
-
-        //   addButtonToToolbar(notebookPanel);
-
-        // });
-        // ////
       }
       catch (e) {
         console.error(e);
       }
     })();
 
     return etcJupyterLabFeedbackServiceFactory;
```

### Comparing `etc_jupyterlab_feedback-2.0.5/src/service.ts` & `etc_jupyterlab_feedback-2.1.0/src/service.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import { Widget } from '@lumino/widgets';
 import { ISignal, Signal } from "@lumino/signaling";
-import { INotebookTracker, Notebook, NotebookPanel, KernelError } from '@jupyterlab/notebook';
-import { INotebookContent } from '@jupyterlab/nbformat';
+import { NotebookPanel, KernelError } from '@jupyterlab/notebook';
 import { requestAPI } from './handler';
 import {
     Cell,
     ICellModel
 } from '@jupyterlab/cells';
 
 import {
     showDialog,
     Dialog
 } from '@jupyterlab/apputils';
 
-import { ETCJupyterLabConfigurableTextButton, IETCJupyterLabConfigurableTextButtonOptions } from './button';
+import { ETCJupyterLabConfigurableTextButton } from './button';
 
 export interface ICellMeta {
     index: number;
     id: any;
 }
 
 export interface INotebookEventMessage {
@@ -99,24 +98,24 @@
                 notebookPanel: this._notebookPanel,
                 cells: cells,
                 message: ''
             });
 
             this._etcJupyterLabConfigurableTextButton.innerHtml = 'Feedback...';
 
-            this._notebookPanel.content.model?.metadata.set(
-                'etc_active_cell',
-                this._notebookPanel.content.activeCellIndex
-            );
+            this._notebookPanel.content.model?.setMetadata(
+                    'etc_active_cell',
+                    this._notebookPanel.content.activeCellIndex
+                );
 
             await this._notebookPanel.context.save();
 
             let feedback = (async () => {
                 try {
-                    if (this._notebookPanel.content.model?.metadata.get('etc_feedback') == true) {
+                    if (this._notebookPanel.content.model?.getMetadata('etc_feedback') == true) {
                         return await requestAPI<any>('feedback', {
                             body: JSON.stringify({
                                 'notebook_path': this._notebookPanel.context.path
                             }),
                             method: 'POST'
                         });
                     }
```

### Comparing `etc_jupyterlab_feedback-2.0.5/tsconfig.json` & `etc_jupyterlab_feedback-2.1.0/tsconfig.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9868421052631579%*

 * *Differences: {"'compilerOptions'": "{'noUnusedLocals': True, 'target': 'ES2018'}"}*

```diff
@@ -6,21 +6,21 @@
         "esModuleInterop": true,
         "incremental": true,
         "jsx": "react",
         "module": "esnext",
         "moduleResolution": "node",
         "noEmitOnError": true,
         "noImplicitAny": true,
-        "noUnusedLocals": false,
+        "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
         "strictNullChecks": true,
-        "target": "es2017",
+        "target": "ES2018",
         "types": []
     },
     "include": [
         "src/*"
     ]
 }
```

