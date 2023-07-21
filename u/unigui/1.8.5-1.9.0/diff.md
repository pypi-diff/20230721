# Comparing `tmp/unigui-1.8.5.tar.gz` & `tmp/unigui-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.8.5.tar", last modified: Wed Jul 19 03:26:32 2023, max compression
+gzip compressed data, was "dist/unigui-1.9.0.tar", last modified: Fri Jul 21 11:09:12 2023, max compression
```

## Comparing `unigui-1.8.5.tar` & `unigui-1.9.0.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-19 03:26:32.000000 unigui-1.8.5/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui/
--rw-rw-r--   0 george    (1000) george    (1000)     8519 2023-07-19 00:31:05.000000 unigui-1.8.5/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)     2744 2023-07-18 23:50:34.000000 unigui-1.8.5/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)      100 2023-07-14 22:20:13.000000 unigui-1.8.5/unigui/__init__.py
--rw-rw-r--   0 george    (1000) george    (1000)     3321 2023-07-18 19:22:00.000000 unigui-1.8.5/unigui/autotest.py
--rw-r--r--   0 george    (1000) george    (1000)     2199 2023-07-18 23:05:47.000000 unigui-1.8.5/unigui/utils.py
--rw-rw-r--   0 george    (1000) george    (1000)     4544 2023-07-18 18:55:27.000000 unigui-1.8.5/unigui/reloader.py
--rw-rw-r--   0 george    (1000) george    (1000)     8612 2023-07-18 22:22:05.000000 unigui-1.8.5/unigui/users.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)   220628 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/css/vendor.191faa77.css
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/css/164.06cedad1.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   128616 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)    45370 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/js/164.2b869daf.js
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)  1434072 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/js/vendor.3076c5e7.js
--rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/js/app.e17901f8.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.8.5/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      612 2023-07-19 03:25:49.000000 unigui-1.8.5/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    19239 2023-07-19 03:26:32.000000 unigui-1.8.5/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-19 03:26:32.000000 unigui-1.8.5/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    18934 2023-07-17 14:52:22.000000 unigui-1.8.5/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.8.5/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       39 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    19239 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.8.5/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1241 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-21 11:09:12.000000 unigui-1.9.0/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-21 11:09:12.000000 unigui-1.9.0/unigui/
+-rw-rw-r--   0 george    (1000) george    (1000)     8595 2023-07-21 05:14:03.000000 unigui-1.9.0/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)     2644 2023-07-21 08:53:12.000000 unigui-1.9.0/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)      108 2023-07-21 04:22:38.000000 unigui-1.9.0/unigui/__init__.py
+-rw-rw-r--   0 george    (1000) george    (1000)     4801 2023-07-21 10:35:37.000000 unigui-1.9.0/unigui/autotest.py
+-rw-r--r--   0 george    (1000) george    (1000)     2490 2023-07-21 10:20:58.000000 unigui-1.9.0/unigui/utils.py
+-rw-rw-r--   0 george    (1000) george    (1000)     5587 2023-07-19 22:23:17.000000 unigui-1.9.0/unigui/reloader.py
+-rw-rw-r--   0 george    (1000) george    (1000)     8110 2023-07-21 04:21:24.000000 unigui-1.9.0/unigui/users.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-21 11:09:12.000000 unigui-1.9.0/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-21 11:09:12.000000 unigui-1.9.0/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)   220628 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/css/vendor.191faa77.css
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)    37826 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/css/vendor.191faa77.css.gz
+-rw-rw-r--   0 george    (1000) george    (1000)     3296 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/css/615.3024385a.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-21 11:09:12.000000 unigui-1.9.0/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-21 11:09:12.000000 unigui-1.9.0/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   128616 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-21 11:09:12.000000 unigui-1.9.0/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)    46024 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/js/615.04cc6ad4.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)  1434072 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/js/vendor.3076c5e7.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/js/app.fb1ab18a.js
+-rw-rw-r--   0 george    (1000) george    (1000)    14198 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/js/615.04cc6ad4.js.gz
+-rw-rw-r--   0 george    (1000) george    (1000)   469734 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/js/vendor.3076c5e7.js.gz
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-21 10:44:37.000000 unigui-1.9.0/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.9.0/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      630 2023-07-21 11:08:25.000000 unigui-1.9.0/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    19239 2023-07-21 11:09:12.000000 unigui-1.9.0/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-21 11:09:12.000000 unigui-1.9.0/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    18934 2023-07-17 14:52:22.000000 unigui-1.9.0/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.9.0/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-21 11:09:12.000000 unigui-1.9.0/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       54 2023-07-21 11:09:12.000000 unigui-1.9.0/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-21 11:09:12.000000 unigui-1.9.0/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    19239 2023-07-21 11:09:12.000000 unigui-1.9.0/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.9.0/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1348 2023-07-21 11:09:12.000000 unigui-1.9.0/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-21 11:09:12.000000 unigui-1.9.0/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.8.5/unigui/guielements.py` & `unigui-1.9.0/unigui/guielements.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 class Tree(Gui):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)         
         self.type = 'tree' 
         if not hasattr(self,'options'):
             self.options = {}        
         if not hasattr(self,'value'):
-            self.value = None
+            self.value = None        
 
 def accept_cell_value(table, val):    
     value, position = val
     if not isinstance(value, bool):
         try:
             value = float(value)        
         except ValueError:
@@ -184,14 +184,16 @@
             self.type = 'table'
         if not hasattr(self,'value'):
             self.value = None
         if not hasattr(self,'rows'):
             self.rows = []
         if not hasattr(self,'value'):
             self.value = None
+        if not hasattr(self,'dense'):
+            self.dense = True
 
         if getattr(self,'edit', True):
             edit_setting = hasattr(self,'modify') or hasattr(self,'delete') or hasattr(self,'append')
             if not edit_setting:                             
                 self.delete = delete_table_row             
                 self.append = append_table_row             
                 self.modify = accept_cell_value
```

### Comparing `unigui-1.8.5/unigui/server.py` & `unigui-1.9.0/unigui/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from aiohttp import web, WSMsgType
 from .users import *
 from pathlib import Path
 from .reloader import empty_app 
-from .autotest import recorder
-from config import port, pretty_print, upload_dir
+from .autotest import recorder, jsonString
+from config import port, upload_dir
 from .utils import app_dir
 import traceback
 
 async def post_handler(request):
     reader = await request.multipart()
     field = await reader.next()   
     filename = upload_path(field.filename)      
@@ -18,17 +18,14 @@
             if not chunk:
                 break
             size += len(chunk)
             f.write(chunk)
 
     return web.Response(text=filename)
 
-def jsonString(obj):
-    return toJson(obj, 2 if pretty_print else 0, pretty_print)
-
 async def static_serve(request):    
     file_path = request.path    
     file_path  = Path(f"{webpath}{file_path}" )
     if request.path == '/':
         file_path /= 'index.html' 
     
     answer = web.HTTPNotFound() if not file_path.exists() else web.FileResponse(file_path)          
@@ -53,23 +50,22 @@
             if msg.type == WSMsgType.TEXT:
                 if msg.data == 'close':
                     await ws.close()
                 else:
                     data = json.loads(msg.data)            
                     result = user.result4message(data)
                     if result:            
-                        result = jsonString(user.prepare_result(result))    
-                        await ws.send_str(result)
-                    recorder(msg.data, result)
+                        result = user.prepare_result(result)
+                        await ws.send_str(jsonString(result))
+                    recorder(data, result)
 
             elif msg.type == WSMsgType.ERROR:
                 print('ws connection closed with exception %s' % ws.exception())
     except:        
         user.log(traceback.format_exc())
-    
     return ws       
 
 def start(appname = '', user_type = User, http_handlers = []):
     if appname:
         config.appname = appname
 
     User.UserType = user_type
```

### Comparing `unigui-1.8.5/unigui/utils.py` & `unigui-1.9.0/unigui/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import os 
-import jsonpickle
-import json
+import os, jsonpickle, json, platform, requests
 
 blocks_dir = 'blocks'        
 screens_dir =  'screens'        
 UpdateScreen = True
 
 libpath = os.path.dirname(os.path.realpath(__file__))
 webpath = libpath + '/web' 
 app_dir = os.getcwd()
+divpath = '\\' if platform.system() == 'Windows' else '/'
 
 try:
     import config
 except:
     with open('config.py', 'w') as f:        
         f.write("""port = 8000 
 upload_dir = 'web'
@@ -20,47 +19,50 @@
 hot_reload   = True
 logfile  = 'log'
 autotest = '*'
 """)
         import config
         print("Config with default parameters is created!")
 
-def toJson(obj, indent, pretty_print):
-    return json.dumps(json.loads(jsonpickle.encode(obj,unpicklable=False)), 
-        indent = indent, sort_keys = pretty_print)
+def toJson(obj, indent, pretty):
+    js = jsonpickle.encode(obj,unpicklable=False)
+    return json.dumps(json.loads(js), indent=indent, sort_keys=pretty) if pretty else js
 
 def filename2url(fn):   
-    if fn[0] == '/':
+    if fn[0] == '/' or fn[1] == ':': #if full path
         fn = fn[len(app_dir):]   
     return fn.replace(' ','%20')
 
-def url2filename(url):
+def url2filepath(url):
     return url[url.find('/') + 1:].replace('%20',' ')   
 
+def url2filename(url):
+    return url[url.rfind('/') + 1:].replace('%20',' ')   
+
 def upload_path(fpath):
-    return f'{config.upload_dir}/{fpath}'
+    return f'{config.upload_dir}{divpath}{fpath}'
 
 def flatten(*arr):
     for a in arr:
         if isinstance(a, list):
             yield from flatten(*a)
         else:
             yield a
-            
-#for registering screen handlers of outer blocks
-handlers__ = {}
-
-def clean_handlers():
-    global handlers__
-    handlers__ = {}
-
-def handle(elem, event):
-    def h(fn):
-        handlers__[elem, event] = fn
-    return h
+    
+def cache_url(url):
+    "cache url file in upload_dir snd returns local file"""
+    fname = url2filename(url)   
+    fname = upload_path(fname)
+    response = requests.get(url)
+    if response.status_code != 200:
+        return None
+    file = open(fname, "wb")
+    file.write(response.content)
+    file.close() 
+    return fname
 
 class Message:
     def __init__(self, *gui_objects, user = None):
         if gui_objects:
             self.updates = [{'data': gui} for gui in gui_objects]
             if user:
                 self.fill_paths4(user)
```

### Comparing `unigui-1.8.5/unigui/users.py` & `unigui-1.9.0/unigui/users.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,80 +1,59 @@
 import importlib
 from .utils import *
 from .guielements import *
 import sys
 import asyncio
-import requests
 from threading import Thread
 import logging
 
 class User:      
     def __init__(self):          
         self.screens = []        
         self.active_dialog = None
-        self.screen_module = None                        
+        self.screen_module = None    
+        self.__handlers__ = {}                    
         User.last_user = self        
 
     def log(self, str, type = 'error'):        
         scr = self.screen.name if self.screens else 'omitted'
         str = f"session: {self.session__}, screen: {scr}, message: {self.message__} \n  {str}"
         if type == 'error':
             logging.error(str)
         else:
             logging.warning(str)
 
-    @staticmethod
-    def cache_name(url):    
-        name = url.split('/')[-1]
-        name = utils.upload_path(name)
-        return name
-        
-    @staticmethod
-    def cache_url(url):
-        "returns cached name of url image"
-        cname = User.cache_name(url)
-        if not os.path.exists(cname):
-            response = requests.get(url)
-            if response.status_code != 200:
-                return None
-            file = open(cname, "wb")
-            file.write(response.content)
-            file.close() 
-        return cname
-
     def sync_send(self, obj):
         asyncio.run_coroutine_threadsafe(self.send(obj), self.extra_loop)            
 
     def progress(self, str, *updates):
         """open or update progress window if str != null else close it  """             
         return self.sync_send(TextMessage('progress', str, *updates, user = self))
-                       
-    def load_module(self, file):
+                   
+    def load_screen(self, file):
         screen_vars = {
             'icon' : None,
             'prepare' : None,            
             'blocks' : [],
             'header' : config.appname,                        
-            'toolbar' : User.toolbar, 
+            'toolbar' : [], 
             'order' : 0
         }             
-        name = file[0:-3]        
+        name = file[:-3]        
         path = f'{screens_dir}/{file}'                
         spec = importlib.util.spec_from_file_location(name,path)
         module = importlib.util.module_from_spec(spec)        
-        
-        utils.clean_handlers()                                        
+                
         module.user = self                               
         
         spec.loader.exec_module(module)            
         screen = Screen(module.name)
         #set system vars
         for var in screen_vars:                                            
-            setattr(screen, var, getattr(module,var,screen_vars[var])) 
-        module.handlers__ = utils.handlers__
+            setattr(screen, var, getattr(module,var,screen_vars[var]))         
         
         if screen.toolbar:
             screen.toolbar += User.toolbar
         else: 
             screen.toolbar = User.toolbar  
                         
         screen.check()                         
@@ -90,15 +69,15 @@
                     if name in sys.modules:
                         sys.modules[name].user = self
                         del sys.modules[name]                          
     def load(self):              
         if os.path.exists(screens_dir):
             for file in os.listdir(screens_dir):
                 if file.endswith(".py") and file != '__init__.py':
-                    module = self.load_module(file)                
+                    module = self.load_screen(file)                
                     self.screens.append(module)                
             
         if self.screens:
             self.screens.sort(key=lambda s: s.screen.order)            
             main = self.screens[0]
             if 'prepare' in dir(main):
                 main.prepare()
@@ -140,28 +119,28 @@
         return result
 
     @property
     def blocks(self):
         return [self.active_dialog.content] if self.active_dialog and \
             self.active_dialog.content else self.screen.blocks
 
-    def find_element(self, path):       
-        if path[0] == 'toolbar':
-            for e in self.screen.toolbar:
-                if e.name == path[1]:                
-                    return e
+    def find_element(self, path):               
         for bl in flatten(self.blocks):
             if bl.name == path[0]:
                 for c in bl.value:
                     if isinstance(c, list):
                         for sub in c:
                             if sub.name == path[1]:
                                 return sub
                     elif c.name == path[1]:
                         return c
+        if path[0] == 'toolbar':
+            for e in self.screen.toolbar:
+                if e.name == path[1]:                
+                    return e
 
     def find_path(self, elem):        
         for bl in flatten(self.blocks):        
             if bl == elem:
                 return [bl.name]
             for c in bl.value:
                 if isinstance(c, list):
@@ -191,49 +170,52 @@
         if arr[0] == 'root':
             for s in self.screens:
                 if s.name == arr[1]:
                     self.screen_module = s
                     if getattr(s.screen,'prepare', False):
                         s.screen.prepare()
                     return True            
-            print(f'Unknown screen name: {s.name}')
+            self.log(f'Unknown screen name: {s.name}')
         else:
             elem = self.find_element(arr)                        
             return self.process_element(elem, arr)        
         
     def process_element(self, elem, arr):        
         id = arr.pop() if len(arr) == 5 else 0
         action = arr[-2]        
         val = arr[-1]
         
-        handler = self.screen_module.handlers__.get((elem, action))
+        handler = self.__handlers__.get((elem, action), None)
         if handler:
             result = handler(elem, val)                
             return result
         
         handler = getattr(elem, action, False)                                
         if handler:                
             res = handler(elem, val)  
             if id:                        
                 res = Answer(res, None, id)                
             return res
         elif action == 'changed':
             if hasattr(elem,'value'): #exlude Buttons and others without 'value'
                 elem.value = val                                        
-            return                        
-
-        return Error(f'{elem} does not contain method for {action} event type!')
+            return   
+        self.log(f'{elem} does not contain method for {action} event type!')                     
+        return Error('Internal server error.')
 
 #loop and thread is for progress window and sync interactions
 loop = asyncio.new_event_loop()
 User.extra_loop = loop
 
 def f(loop):
     asyncio.set_event_loop(loop)
     loop.run_forever() 
-    
-async_thread = Thread(target=f, args=(loop,))
-async_thread.start()  
 
-User.toolbar = []
+async_thread = Thread(target=f, args=(loop,))
+async_thread.start()
 
+def handle(elem, event):
+    def h(fn):
+        User.last_user.__handlers__[elem, event] = fn
+    return h
 
+User.toolbar = []
```

### Comparing `unigui-1.8.5/unigui/web/favicon.ico` & `unigui-1.9.0/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.8.5/unigui/web/css/vendor.191faa77.css` & `unigui-1.9.0/unigui/web/css/vendor.191faa77.css`

 * *Files identical despite different names*

### Comparing `unigui-1.8.5/unigui/web/css/164.06cedad1.css` & `unigui-1.9.0/unigui/web/css/615.3024385a.css`

 * *Files 11% similar despite different names*

```diff
@@ -1 +1 @@
-thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-7eaff898]{display:flex;justify-content:center}.custom-caption[data-v-7eaff898]{padding:5px!important}.web-camera-container[data-v-7eaff898]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-7eaff898]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-7eaff898]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-7eaff898]{opacity:1}.web-camera-container .camera-shoot[data-v-7eaff898]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-7eaff898]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-7eaff898]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-7eaff898]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-7eaff898]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-7eaff898]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-7eaff898]{animation:preload-7eaff898 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-7eaff898]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-7eaff898]:nth-child(3){animation-delay:.4s}@keyframes preload-7eaff898{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-7eaff898]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
+thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-9259610c]{display:flex;justify-content:center}.custom-caption[data-v-9259610c]{padding:5px!important}.web-camera-container[data-v-9259610c]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-9259610c]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-9259610c]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-9259610c]{opacity:1}.web-camera-container .camera-shoot[data-v-9259610c]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-9259610c]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-9259610c]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-9259610c]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-9259610c]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-9259610c]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-9259610c]{animation:preload-9259610c 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-9259610c]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-9259610c]:nth-child(3){animation-delay:.4s}@keyframes preload-9259610c{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-9259610c]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}.invisible{visibility:hidden}
```

### Comparing `unigui-1.8.5/unigui/web/icons/favicon-96x96.png` & `unigui-1.9.0/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.8.5/unigui/web/icons/favicon-16x16.png` & `unigui-1.9.0/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.8.5/unigui/web/icons/favicon-32x32.png` & `unigui-1.9.0/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.8.5/unigui/web/icons/favicon-128x128.png` & `unigui-1.9.0/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.8.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2` & `unigui-1.9.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.8.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.9.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.5/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.9.0/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.5/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.9.0/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.5/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.9.0/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.5/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.9.0/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.5/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.9.0/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.5/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.9.0/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.5/unigui/web/js/164.2b869daf.js` & `unigui-1.9.0/unigui/web/js/615.04cc6ad4.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [164], {
-        4164: (e, t, a) => {
+    [615], {
+        9615: (e, t, a) => {
             a.r(t), a.d(t, {
-                default: () => ea
+                default: () => sa
             });
             var l = a(3673),
                 s = a(2323);
             const i = (0, l._)("div", {
                     class: "q-pa-lg"
                 }, null, -1),
                 n = (0, l._)("div", {
@@ -74,15 +74,16 @@
                         })])),
                         _: 1
                     }), (0, l.Wm)(w, null, {
                         default: (0, l.w5)((() => [(0, l.Wm)(y, {
                             class: "flex justify-center centers"
                         }, {
                             default: (0, l.w5)((() => [(0, l.Wm)(f, {
-                                data: e.screen.blocks
+                                data: e.screen.blocks,
+                                ref: "page"
                             }, null, 8, ["data"])])),
                             _: 1
                         })])),
                         _: 1
                     })])),
                     _: 1
                 })
@@ -133,89 +134,100 @@
                 return `height: ${t}px; width: ${a}px`
             }
             const b = window.location.host,
                 k = `${window.location.protocol}//${b}`;
             console.log(k);
             const v = !1;
             let C = {},
-                q = {};
+                q = {},
+                _ = {};
 
-            function _(e) {
+            function j(e) {
                 p = new WebSocket(v ? "ws://localhost:8000/ws" : `ws://${b}/ws`), p.onopen = () => e.statusConnect = !0, p.onmessage = t => {
                     g && console.log("incoming message", t.data), e.processMessage(JSON.parse(t.data))
                 }, p.onerror = t => e.error(t), p.onclose = t => {
                     t.wasClean ? e.info("Connection was finished by the server.") : e.error("Connection suddenly closed!"), e.statusConnect = !1, g && console.info("close code : " + t.code + " reason: " + t.reason)
                 }, h = e
             }
 
-            function j(e) {
+            function S(e) {
                 console.log("sended", e), p.send(JSON.stringify(e))
             }
-            let S, z = 0;
+            let z, A = 0,
+                Z = !0;
 
-            function A() {
-                for (let [e, t] of Object.entries(q)) t.styleSize = null
+            function $(e) {
+                Z = e, e || (_ = {})
             }
 
-            function Z(e, t, a, l = "complete") {
-                let s = ++z,
+            function D(e, t) {
+                if (Z) {
+                    let t = _[e];
+                    if (t) return t.styleSize;
+                    Z = !1
+                }
+                return w(t)
+            }
+
+            function M(e, t, a, l = "complete") {
+                let s = ++A,
                     i = [e.pdata.name, e.data.name, l, t, s];
-                j(i), u[s] = a
+                S(i), u[s] = a
             }
 
-            function D() {
-                C = {}, q = {}
+            function V() {
+                C = {}, _ = q, Z = !0, q = {}
             }
 
-            function M(e, t) {
+            function E(e, t) {
                 Object.assign(e.data, t), e.updated = t.value, e.value = t.value
             }
 
-            function $(e) {
+            function K(e) {
                 for (let t of e) {
                     let e = t.path;
                     if (e.length > 1) {
                         e.reverse();
                         let a = e.join("@"),
                             l = q[a];
-                        M(l, t.data)
+                        E(l, t.data)
                     } else {
                         let a = C[e[0]];
                         Object.assign(a.data, t.data)
                     }
                 }
             }
 
-            function V(e) {
+            function W(e) {
                 "string" == typeof e.value ? h.error(e.value) : u[e.id](e.value), delete u[e.id]
             }
 
-            function E(e) {
+            function O(e) {
                 let t = [];
                 for (let l of e) l instanceof Array ? t.push(l) : t.push([l]);
                 let a = t.shift();
                 return t.reduce(((e, t) => e.flatMap((e => t.map((t => e instanceof Array ? [...e, t] : [e, t]))))), a)
             }
 
-            function K() {
+            function Q() {
                 for (let [e, t] of Object.entries(q)) t.expanding && (t.styleSize = w(t.data));
                 (0, l.Y3)((() => {
                     requestAnimationFrame((() => {
                         requestAnimationFrame((() => {
-                            O()
+                            U()
                         }))
                     }))
                 }))
             }
-            let W = (0, c.debounce)(K, 200);
+            let H = (0, c.debounce)(Q, 200);
 
-            function O(e) {
-                Array.isArray(e) && (e = null), S && (S.disconnect(), S = null), g && console.log("------------------recalc design");
-                const t = Q(e),
-                    a = H(e);
+            function U(e) {
+                Array.isArray(e) && (e = null), z && (z.disconnect(), z = null), g && console.log("------------------recalc design");
+                const t = N(e),
+                    a = F(e);
                 for (let [l, s] of Object.entries(t)) {
                     let e = q[l];
                     const [t, i] = a[l];
                     let n, o = e.geom().el,
                         d = e.pdata ? e.pdata.name : e.name,
                         r = C[d];
                     for (let a of r.data.value.slice(1))
@@ -233,27 +245,27 @@
                     let c = r.data.width ? r.data.width - o.clientWidth - t : r.$el.getBoundingClientRect().right - (n ? n.geom().right : e.geom().right);
                     c /= i;
                     let h = l.startsWith("_scroll@") ? e.geom().inner.clientHeight : o.clientHeight;
                     e.styleSize = `height: ${h+s}px; width: ${o.clientWidth+c+t}px;`
                 }
             }
 
-            function Q(e) {
+            function N(e) {
                 const t = h.screen.blocks;
                 let a = window.innerHeight;
-                a -= 2;
+                a += 5;
                 let l = {},
                     s = new Map,
                     i = {};
                 for (let [d, r] of Object.entries(C)) i[r.name] = r.$el.getBoundingClientRect().height;
                 let n = [];
                 for (let d of t) {
                     const e = [];
                     let t = d instanceof Array,
-                        o = t ? E(d) : [
+                        o = t ? O(d) : [
                             [d]
                         ];
                     for (let a of o) {
                         let e = 0;
                         for (let t of a) e += i[t.name] + 8;
                         n.push([e, a])
                     }
@@ -299,18 +311,18 @@
                 }
                 let o = Array.from(s.entries());
                 o.sort(((e, t) => e[0] in l || e[1] in l ? -1 : 1));
                 for (let [d, r] of o) r in l ? l[d] = l[r] : l[r] = l[d];
                 return l
             }
 
-            function H(e) {
+            function F(e) {
                 e = null;
                 const t = e ? [e] : h.screen.blocks;
-                let a = window.innerWidth - 30,
+                let a = window.innerWidth - 15,
                     l = [],
                     s = {};
                 for (let o of t)
                     if (0 == l.length)
                         if (Array.isArray(o))
                             for (let e of o) l.push(Array.isArray(e) ? e : [e]);
                         else l = [
@@ -379,198 +391,198 @@
                             s[a.fullname] = [Math.floor(o / e), t[l]]
                         }
                     }
                 }
                 for (let [o, d] of n.entries()) d in s ? s[o] = s[d] : s[d] = s[o];
                 return s
             }
-            const U = (0, l.aZ)({
+            const T = (0, l.aZ)({
                 name: "menubar",
                 methods: {
                     send() {
-                        j(["root", this.name])
+                        S(["root", this.name])
                     }
                 },
                 props: {
                     name: {
                         type: String,
                         required: !0
                     },
                     icon: {
                         type: String,
                         default: ""
                     }
                 }
             });
-            var N = a(4260),
-                F = a(3414),
-                T = a(2035),
-                P = a(4554),
-                I = a(2350),
-                R = a(7518),
-                L = a.n(R);
-            const B = (0, N.Z)(U, [
+            var P = a(4260),
+                R = a(3414),
+                I = a(2035),
+                L = a(4554),
+                B = a(2350),
+                Y = a(7518),
+                X = a.n(Y);
+            const G = (0, P.Z)(T, [
                     ["render", d]
                 ]),
-                Y = B;
-            L()(U, "components", {
-                QItem: F.Z,
-                QItemSection: T.Z,
-                QIcon: P.Z,
-                QItemLabel: I.Z
+                J = G;
+            X()(T, "components", {
+                QItem: R.Z,
+                QItemSection: I.Z,
+                QIcon: L.Z,
+                QItemLabel: B.Z
             });
-            const X = {
+            const ee = {
                     key: 0,
                     class: "row q-col-gutter-sm q-py-sm"
                 },
-                G = {
+                te = {
                     class: "q-col-gutter-sm"
                 },
-                J = {
+                ae = {
                     key: 0,
                     class: "column q-col-gutter-sm"
                 };
 
-            function ee(e, t, a, s, i, n) {
+            function le(e, t, a, s, i, n) {
                 const o = (0, l.up)("zone", !0),
                     d = (0, l.up)("block");
-                return e.data instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", X, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data, (e => ((0, l.wg)(), (0, l.iD)("div", G, [e instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", J, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e, (e => ((0, l.wg)(), (0, l.j4)(o, {
+                return e.data instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", ee, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data, (e => ((0, l.wg)(), (0, l.iD)("div", te, [e instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", ae, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e, (e => ((0, l.wg)(), (0, l.j4)(o, {
                     data: e
                 }, null, 8, ["data"])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                     key: 1,
                     data: e
                 }, null, 8, ["data"]))])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                     key: 1,
                     data: e.data
                 }, null, 8, ["data"]))
             }
-            const te = {
+            const se = {
                     class: "row"
                 },
-                ae = {
+                ie = {
                     key: 2,
                     class: "q-ma-sm",
                     style: {
                         "font-size": "18px"
                     }
                 },
-                le = ["data", "pdata"],
-                se = {
+                ne = ["data", "pdata"],
+                oe = {
                     key: 0,
                     class: "row"
                 },
-                ie = ["data", "pdata"],
-                ne = {
+                de = ["data", "pdata"],
+                re = {
                     key: 0,
                     class: "row"
                 };
 
-            function oe(e, t, a, i, n, o) {
+            function ce(e, t, a, i, n, o) {
                 const d = (0, l.up)("element"),
                     r = (0, l.up)("q-icon"),
                     c = (0, l.up)("q-scroll-area"),
                     h = (0, l.up)("q-card");
                 return (0, l.wg)(), (0, l.j4)(h, {
                     class: "my-card q-ma-xs"
                 }, {
-                    default: (0, l.w5)((() => [(0, l._)("div", te, [e.data.logo ? ((0, l.wg)(), (0, l.j4)(d, {
+                    default: (0, l.w5)((() => [(0, l._)("div", se, [e.data.logo ? ((0, l.wg)(), (0, l.j4)(d, {
                         key: 0,
                         data: e.data.logo,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])) : e.data.icon ? ((0, l.wg)(), (0, l.j4)(r, {
                         key: 1,
                         size: "sm",
                         name: e.data.icon
-                    }, null, 8, ["name"])) : (0, l.kq)("", !0), "_" != e.name[0] ? ((0, l.wg)(), (0, l.iD)("p", ae, (0, s.zw)(e.name), 1)) : (0, l.kq)("", !0), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.tops, (t => ((0, l.wg)(), (0, l.j4)(d, {
+                    }, null, 8, ["name"])) : (0, l.kq)("", !0), "_" != e.name[0] ? ((0, l.wg)(), (0, l.iD)("p", ie, (0, s.zw)(e.name), 1)) : (0, l.kq)("", !0), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.tops, (t => ((0, l.wg)(), (0, l.j4)(d, {
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])))), 256))]), e.data.scroll ? ((0, l.wg)(), (0, l.j4)(c, {
                         key: 0,
                         style: (0, s.j5)(e.styleSize),
                         "thumb-style": e.thumbStyle,
                         "bar-style": e.barStyle
                     }, {
                         default: (0, l.w5)((() => [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data.value.slice(1), (t => ((0, l.wg)(), (0, l.iD)("div", {
                             class: "column",
                             data: t,
                             pdata: e.data
-                        }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", se, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
+                        }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", oe, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
                             class: "q-ma-xs",
                             data: t,
                             pdata: e.data
                         }, null, 8, ["data", "pdata"])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                             key: 1,
                             class: "q-ma-xs",
                             data: t,
                             pdata: e.data
-                        }, null, 8, ["data", "pdata"]))], 8, le)))), 256))])),
+                        }, null, 8, ["data", "pdata"]))], 8, ne)))), 256))])),
                         _: 1
                     }, 8, ["style", "thumb-style", "bar-style"])) : ((0, l.wg)(!0), (0, l.iD)(l.HY, {
                         key: 1
                     }, (0, l.Ko)(e.data.value.slice(1), (t => ((0, l.wg)(), (0, l.iD)("div", {
                         class: "column",
                         data: t,
                         pdata: e.data
-                    }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", ne, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
+                    }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", re, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                         key: 1,
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
-                    }, null, 8, ["data", "pdata"]))], 8, ie)))), 256))])),
+                    }, null, 8, ["data", "pdata"]))], 8, de)))), 256))])),
                     _: 1
                 })
             }
-            var de = a(8880);
-            const re = e => ((0, l.dD)("data-v-7eaff898"), e = e(), (0, l.Cn)(), e),
-                ce = {
+            var he = a(8880);
+            const ue = e => ((0, l.dD)("data-v-9259610c"), e = e(), (0, l.Cn)(), e),
+                pe = {
                     key: 4
                 },
-                he = ["width", "height"],
-                ue = ["src"],
-                pe = {
+                ge = ["width", "height"],
+                me = ["src"],
+                fe = {
                     key: 17,
                     class: "web-camera-container"
                 },
-                ge = {
+                ye = {
                     class: "camera-button"
                 },
-                me = {
+                we = {
                     key: 0
                 },
-                fe = {
+                be = {
                     key: 1
                 },
-                ye = {
+                ke = {
                     class: "camera-loading"
                 },
-                we = re((() => (0, l._)("ul", {
+                ve = ue((() => (0, l._)("ul", {
                     class: "loader-circle"
                 }, [(0, l._)("li"), (0, l._)("li"), (0, l._)("li")], -1))),
-                be = [we],
-                ke = ["height"],
-                ve = ["height"],
-                xe = {
+                xe = [ve],
+                Ce = ["height"],
+                qe = ["height"],
+                _e = {
                     key: 1,
                     class: "camera-shoot"
                 },
-                Ce = re((() => (0, l._)("img", {
+                je = ue((() => (0, l._)("img", {
                     src: "https://img.icons8.com/material-outlined/50/000000/camera--v2.png"
                 }, null, -1))),
-                qe = [Ce],
-                _e = {
+                Se = [je],
+                ze = {
                     key: 2,
                     class: "camera-download"
                 };
 
-            function je(e, t, a, i, n, o) {
+            function Ae(e, t, a, i, n, o) {
                 const d = (0, l.up)("q-icon"),
                     r = (0, l.up)("q-img"),
                     c = (0, l.up)("q-badge"),
                     h = (0, l.up)("q-select"),
                     u = (0, l.up)("q-checkbox"),
                     p = (0, l.up)("q-toggle"),
                     g = (0, l.up)("q-btn"),
@@ -585,22 +597,22 @@
                     C = (0, l.up)("cgraph"),
                     q = (0, l.up)("q-tooltip"),
                     _ = (0, l.up)("q-spinner-puff");
                 return "image" == e.type ? ((0, l.wg)(), (0, l.j4)(r, {
                     key: 0,
                     src: e.data.name,
                     "spinner-color": "blue",
-                    onClick: (0, de.iM)(e.switchValue, ["stop"]),
+                    onClick: (0, he.iM)(e.switchValue, ["stop"]),
                     fit: "cover",
                     style: (0, s.j5)(e.elemSize)
                 }, {
                     default: (0, l.w5)((() => [e.data.header ? ((0, l.wg)(), (0, l.iD)("div", {
                         key: 0,
                         class: "absolute-bottom-right text-subtitle2 custom-caption",
-                        onClick: t[0] || (t[0] = (0, de.iM)(((...t) => e.lens && e.lens(...t)), ["stop"]))
+                        onClick: t[0] || (t[0] = (0, he.iM)(((...t) => e.lens && e.lens(...t)), ["stop"]))
                     }, (0, s.zw)(e.data.header), 1)) : (0, l.kq)("", !0), e.value ? ((0, l.wg)(), (0, l.j4)(d, {
                         key: 1,
                         class: "absolute all-pointer-events",
                         size: "32px",
                         name: "check_circle",
                         color: "light-blue-2",
                         style: {
@@ -640,15 +652,15 @@
                 }, null, 8, ["modelValue", "label"])) : "switch" == e.type ? ((0, l.wg)(), (0, l.j4)(p, {
                     key: 3,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[3] || (t[3] = t => e.value = t),
                     color: "primary",
                     label: e.nameLabel,
                     "left-label": ""
-                }, null, 8, ["modelValue", "label"])) : "radio" == e.type ? ((0, l.wg)(), (0, l.iD)("div", ce, [e.showname ? ((0, l.wg)(), (0, l.j4)(g, {
+                }, null, 8, ["modelValue", "label"])) : "radio" == e.type ? ((0, l.wg)(), (0, l.iD)("div", pe, [e.showname ? ((0, l.wg)(), (0, l.j4)(g, {
                     key: 0,
                     ripple: !1,
                     color: "secondary",
                     disable: "",
                     label: e.name,
                     "no-caps": ""
                 }, null, 8, ["label"])) : (0, l.kq)("", !0), (0, l.Wm)(m, {
@@ -673,27 +685,27 @@
                     key: 7,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[5] || (t[5] = t => e.value = t),
                     label: e.name,
                     ref: "inputRef",
                     autogrow: e.data.autogrow,
                     dense: "",
-                    onKeyup: (0, de.D2)(e.pressedEnter, ["enter"]),
+                    onKeyup: (0, he.D2)(e.pressedEnter, ["enter"]),
                     readonly: !1 === e.data.edit
                 }, null, 8, ["modelValue", "label", "autogrow", "onKeyup", "readonly"])) : "number" == e.type ? ((0, l.wg)(), (0, l.j4)(w, {
                     key: 8,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[6] || (t[6] = t => e.value = t),
                     modelModifiers: {
                         number: !0
                     },
                     label: e.name,
                     ref: "inputRef",
                     dense: "",
-                    onKeyup: (0, de.D2)(e.pressedEnter, ["enter"]),
+                    onKeyup: (0, he.D2)(e.pressedEnter, ["enter"]),
                     type: "number",
                     readonly: !1 === e.data.edit
                 }, null, 8, ["modelValue", "label", "onKeyup", "readonly"])) : "autoedit" == e.type ? ((0, l.wg)(), (0, l.j4)(h, {
                     key: 9,
                     dense: "",
                     modelValue: e.value,
                     "onUpdate:modelValue": t[7] || (t[7] = t => e.value = t),
@@ -703,53 +715,54 @@
                     outlined: "",
                     "hide-bottom-space": "",
                     "fill-input": "",
                     "input-debounce": "0",
                     options: e.options,
                     onFilter: e.complete,
                     label: e.name,
-                    onKeyup: (0, de.D2)(e.pressedEnter, ["enter"])
+                    onKeyup: (0, he.D2)(e.pressedEnter, ["enter"])
                 }, null, 8, ["modelValue", "options", "onFilter", "label", "onKeyup"])) : "tree" == e.type || "list" == e.type ? ((0, l.wg)(), (0, l.j4)(k, {
                     key: 10,
                     style: (0, s.j5)(e.styleSize),
                     "thumb-style": e.thumbStyle,
                     "bar-style": e.barStyle
                 }, {
                     default: (0, l.w5)((() => [(0, l.Wm)(b, {
                         nodes: e.treeNodes,
+                        dense: e.data.dense,
                         selected: e.value,
                         "onUpdate:selected": t[8] || (t[8] = t => e.value = t),
                         expanded: e.expandedKeys,
                         "onUpdate:expanded": t[9] || (t[9] = t => e.expandedKeys = t),
                         "node-key": "label",
                         "default-expand-all": "",
                         "selected-color": "blue-10"
-                    }, null, 8, ["nodes", "selected", "expanded"])])),
+                    }, null, 8, ["nodes", "dense", "selected", "expanded"])])),
                     _: 1
                 }, 8, ["style", "thumb-style", "bar-style"])) : "docviewer" == e.type ? (0, l.wy)(((0, l.wg)(), (0, l.iD)("textarea", {
                     key: 11,
                     class: "textarea",
                     "onUpdate:modelValue": t[10] || (t[10] = t => e.value = t),
                     filled: "",
                     type: "textarea",
                     style: (0, s.j5)(e.elemSize)
                 }, null, 4)), [
-                    [de.nr, e.value]
+                    [he.nr, e.value]
                 ]) : "line" == e.type ? ((0, l.wg)(), (0, l.j4)(v, {
                     key: 12,
                     color: "green"
                 })) : "video" == e.type ? ((0, l.wg)(), (0, l.iD)("video", {
                     width: e.data.width,
                     height: e.data.height,
                     key: e.data.src,
                     controls: ""
                 }, [(0, l._)("source", {
                     src: e.data.src,
                     type: "video/mp4"
-                }, null, 8, ue)], 8, he)) : "uploader" == e.type ? ((0, l.wg)(), (0, l.j4)(x, {
+                }, null, 8, me)], 8, ge)) : "uploader" == e.type ? ((0, l.wg)(), (0, l.j4)(x, {
                     key: 14,
                     label: e.name,
                     "auto-upload": "",
                     thumbnails: "",
                     url: e.host_path,
                     onUploaded: e.updateDom,
                     onAdded: e.onAdded,
@@ -767,53 +780,53 @@
                     ref: "uploaderRef",
                     flat: ""
                 }, null, 8, ["label", "url", "onUploaded", "onAdded"])) : "graph" == e.type ? ((0, l.wg)(), (0, l.j4)(C, {
                     key: 16,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.elemSize
-                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, l.wg)(), (0, l.iD)("div", pe, [(0, l._)("div", ge, [(0, l._)("button", {
+                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, l.wg)(), (0, l.iD)("div", fe, [(0, l._)("div", ye, [(0, l._)("button", {
                     class: (0, s.C_)(["button is-rounded", {
                         "is-primary": !e.isCameraOpen,
                         "is-danger": e.isCameraOpen
                     }]),
                     type: "button",
                     onClick: t[11] || (t[11] = (...t) => e.toggleCamera && e.toggleCamera(...t))
-                }, [e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("span", fe, "Close Camera")) : ((0, l.wg)(), (0, l.iD)("span", me, "Open Camera"))], 2)]), (0, l.wy)((0, l._)("div", ye, be, 512), [
-                    [de.F8, e.isCameraOpen && e.isLoading]
+                }, [e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("span", be, "Close Camera")) : ((0, l.wg)(), (0, l.iD)("span", we, "Open Camera"))], 2)]), (0, l.wy)((0, l._)("div", ke, xe, 512), [
+                    [he.F8, e.isCameraOpen && e.isLoading]
                 ]), e.isCameraOpen ? (0, l.wy)(((0, l.wg)(), (0, l.iD)("div", {
                     key: 0,
                     class: (0, s.C_)(["camera-box", {
                         flash: e.isShotPhoto
                     }])
                 }, [(0, l._)("div", {
                     class: (0, s.C_)(["camera-shutter", {
                         flash: e.isShotPhoto
                     }])
                 }, null, 2), (0, l.wy)((0, l._)("video", {
                     ref: "camera",
                     width: 450,
                     height: 337.5,
                     autoplay: ""
-                }, null, 8, ke), [
-                    [de.F8, !e.isPhotoTaken]
+                }, null, 8, Ce), [
+                    [he.F8, !e.isPhotoTaken]
                 ]), (0, l.wy)((0, l._)("canvas", {
                     id: "photoTaken",
                     ref: "canvas",
                     width: 450,
                     height: 337.5
-                }, null, 8, ve), [
-                    [de.F8, e.isPhotoTaken]
+                }, null, 8, qe), [
+                    [he.F8, e.isPhotoTaken]
                 ])], 2)), [
-                    [de.F8, !e.isLoading]
-                ]) : (0, l.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, l.wg)(), (0, l.iD)("div", xe, [(0, l._)("button", {
+                    [he.F8, !e.isLoading]
+                ]) : (0, l.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, l.wg)(), (0, l.iD)("div", _e, [(0, l._)("button", {
                     class: "button",
                     type: "button",
                     onClick: t[12] || (t[12] = (...t) => e.takePhoto && e.takePhoto(...t))
-                }, qe)])) : (0, l.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("div", _e, [(0, l.Wm)(g, {
+                }, Se)])) : (0, l.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("div", ze, [(0, l.Wm)(g, {
                     onClick: e.downloadImage,
                     label: "Send"
                 }, null, 8, ["onClick"])])) : (0, l.kq)("", !0)])) : "" != e.showname ? ((0, l.wg)(), (0, l.j4)(g, {
                     key: 18,
                     "no-caps": "",
                     label: e.name,
                     icon: e.data.icon,
@@ -856,37 +869,37 @@
                     }, {
                         default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(e.data.tooltip), 1)])),
                         _: 1
                     })) : (0, l.kq)("", !0)])),
                     _: 1
                 }, 8, ["icon", "onClick"]))
             }
-            const Se = {
+            const Ze = {
                     key: 0
                 },
-                ze = {
+                $e = {
                     class: "row"
                 },
-                Ae = ["onClick"];
+                De = ["onClick"];
 
-            function Ze(e, t, a, i, n, o) {
+            function Me(e, t, a, i, n, o) {
                 const d = (0, l.up)("q-icon"),
                     r = (0, l.up)("q-tooltip"),
                     c = (0, l.up)("q-input"),
                     h = (0, l.up)("q-btn"),
                     u = (0, l.up)("q-th"),
                     p = (0, l.up)("q-tr"),
                     g = (0, l.up)("q-checkbox"),
                     m = (0, l.up)("q-select"),
                     f = (0, l.up)("q-td"),
                     y = (0, l.up)("q-table");
                 return (0, l.wg)(), (0, l.j4)(y, {
                     class: "my-sticky-virtscroll-table",
                     "virtual-scroll": "",
-                    dense: "",
+                    dense: e.data.dense,
                     style: (0, s.j5)(e.styleSize),
                     flat: "",
                     filter: e.search,
                     ref: "table",
                     virtualScrollSliceSize: "60",
                     "rows-per-page-options": [0],
                     "virtual-scroll-sticky-size-start": 48,
@@ -894,15 +907,15 @@
                     title: e.name,
                     rows: e.rows,
                     columns: e.columns,
                     selection: e.singleMode ? "single" : "multiple",
                     selected: e.selected,
                     "onUpdate:selected": t[2] || (t[2] = t => e.selected = t)
                 }, {
-                    "top-right": (0, l.w5)((() => [!1 !== e.data.tools ? ((0, l.wg)(), (0, l.iD)("div", Se, [(0, l._)("div", ze, [(0, l.Wm)(c, {
+                    "top-right": (0, l.w5)((() => [!1 !== e.data.tools ? ((0, l.wg)(), (0, l.iD)("div", Ze, [(0, l._)("div", $e, [(0, l.Wm)(c, {
                         modelValue: e.search,
                         "onUpdate:modelValue": t[1] || (t[1] = t => e.search = t),
                         label: "Search",
                         dense: "",
                         ref: "searchField"
                     }, (0, l.Nv)({
                         append: (0, l.w5)((() => ["" != e.search ? ((0, l.wg)(), (0, l.j4)(d, {
@@ -1083,34 +1096,34 @@
                                 "onUpdate:modelValue": [e => t.row[a.name] = e, e.change],
                                 dense: "",
                                 onKeydown: e.keyInput,
                                 autofocus: ""
                             }, null, 8, ["modelValue", "onUpdate:modelValue", "onKeydown"])) : ((0, l.wg)(), (0, l.iD)("div", {
                                 key: 3,
                                 onClick: a => e.select(t.row.iiid, i)
-                            }, (0, s.zw)(t.row[a.name]), 9, Ae))])),
+                            }, (0, s.zw)(t.row[a.name]), 9, De))])),
                             _: 2
                         }, 1032, ["props"])))), 128))])),
                         _: 2
                     }, 1032, ["props", "onClick"])])),
                     _: 1
-                }, 8, ["style", "filter", "title", "rows", "columns", "selection", "selected"])
+                }, 8, ["dense", "style", "filter", "title", "rows", "columns", "selection", "selected"])
             }
-            var De = a(1959);
+            var Ve = a(1959);
 
-            function Me(e, t) {
+            function Ee(e, t) {
                 return e.length === t.length && e.every(((e, a) => e.iiid == t[a].iiid))
             }
-            const $e = (0, l.aZ)({
+            const Ke = (0, l.aZ)({
                 name: "utable",
                 setup(e) {
                     const {
                         data: t,
                         pdata: a
-                    } = (0, De.BK)(e);
+                    } = (0, Ve.BK)(e);
                     let s = (0, l.Fl)((() => {
                             let e = [],
                                 a = t.value;
                             const l = a.headers,
                                 s = l.length,
                                 i = a.rows,
                                 n = i.length;
@@ -1124,19 +1137,19 @@
                         })),
                         i = () => {
                             let e = t.value,
                                 a = null === e.value || 0 == s.value.length ? [] : Array.isArray(e.value) ? e.value.map((e => s.value[e])) : [s.value[e.value]];
                             return a
                         },
                         n = i(),
-                        o = (0, De.iH)(n),
-                        d = (0, De.iH)(n),
-                        r = (0, De.iH)(!Array.isArray(t.value.value)),
+                        o = (0, Ve.iH)(n),
+                        d = (0, Ve.iH)(n),
+                        r = (0, Ve.iH)(!Array.isArray(t.value.value)),
                         c = (e, l) => {
-                            j([a.value.name, t.value.name, e, l])
+                            S([a.value.name, t.value.name, e, l])
                         },
                         h = (0, l.Fl)((() => r.value ? d.value.length > 0 ? d.value[0].iiid : null : d.value.map((e => e.iiid)))),
                         u = (0, l.Fl)((() => t.value.value));
                     return (0, l.YP)(s, ((e, t) => {
                         d.value = i(), o.value = d.value
                     })), (0, l.YP)(t, ((e, a) => {
                         g && console.log("data update", a.name), d.value = i(), o.value = d.value, r.value = !Array.isArray(t.value.value)
@@ -1225,23 +1238,23 @@
                                         a = typeof t.rows[e][this.cedit];
                                     "string" != a && "number" != a || (t.value = e), this.selected = [this.rows[e]]
                                 }
                                 break
                         }
                     },
                     complete(e, t, a) {
-                        Z(this, [e, [this.redit, this.cedit]], (e => t((() => {
+                        M(this, [e, [this.redit, this.cedit]], (e => t((() => {
                             this.options = e
                         }))))
                     },
                     append() {
                         let e = this.data.rows,
                             t = e.length,
                             a = this;
-                        Z(this, [t, this.search], (function(l) {
+                        M(this, [t, this.search], (function(l) {
                             if (!Array.isArray(l)) return h.error(l);
                             g && console.log("added row", l), a.search = "", e.push(l), setTimeout((() => {
                                 let e = a.rows;
                                 a.selected = [e[t]], a.showSelected(), a.editMode || a.switchEdit(), a.select(e[t], 0)
                             }), 100)
                         }), "append")
                     },
@@ -1276,15 +1289,15 @@
                         }
                         this.selected = []
                     }
                 },
                 watch: {
                     selected(e) {
                         const t = this.data;
-                        if (!Me(this.updated, this.selected)) {
+                        if (!Ee(this.updated, this.selected)) {
                             let e = this.selected.length;
                             this.sendMessage("changed", this.singleMode ? 1 == e ? this.selected[0].iiid : null : this.selected.map((e => e.iiid))), this.updated = this.selected
                         }
                         t.show && (this.showSelected(), t.show = !1), this.editMode && this.selected.length && (t.value = this.selected[0].iiid)
                     }
                 },
                 computed: {
@@ -1309,52 +1322,52 @@
                 },
                 props: {
                     data: Object,
                     pdata: Object,
                     styleSize: String
                 }
             });
-            var Ve = a(9267),
-                Ee = a(4842),
-                Ke = a(8870),
-                We = a(2165),
-                Oe = a(8186),
-                Qe = a(2414),
-                He = a(3884),
-                Ue = a(5735),
-                Ne = a(7208);
-            const Fe = (0, N.Z)($e, [
-                    ["render", Ze]
+            var We = a(9267),
+                Oe = a(4842),
+                Qe = a(8870),
+                He = a(2165),
+                Ue = a(8186),
+                Ne = a(2414),
+                Fe = a(3884),
+                Te = a(5735),
+                Pe = a(7208);
+            const Re = (0, P.Z)(Ke, [
+                    ["render", Me]
                 ]),
-                Te = Fe;
-            L()($e, "components", {
-                QTable: Ve.Z,
-                QInput: Ee.Z,
-                QIcon: P.Z,
-                QTooltip: Ke.Z,
-                QBtn: We.Z,
-                QTr: Oe.Z,
-                QTh: Qe.Z,
-                QTd: He.Z,
-                QCheckbox: Ue.Z,
-                QSelect: Ne.Z
+                Ie = Re;
+            X()(Ke, "components", {
+                QTable: We.Z,
+                QInput: Oe.Z,
+                QIcon: L.Z,
+                QTooltip: Qe.Z,
+                QBtn: He.Z,
+                QTr: Ue.Z,
+                QTh: Ne.Z,
+                QTd: Fe.Z,
+                QCheckbox: Te.Z,
+                QSelect: Pe.Z
             });
-            const Pe = ["nodes", "edges"];
+            const Le = ["nodes", "edges"];
 
-            function Ie(e, t, a, i, n, o) {
+            function Be(e, t, a, i, n, o) {
                 return (0, l.wg)(), (0, l.iD)("div", {
                     nodes: e.nodes,
                     edges: e.edges,
                     style: (0, s.j5)(e.styleSize),
                     ref: "cy"
-                }, null, 12, Pe)
+                }, null, 12, Le)
             }
-            var Re = a(2393),
-                Le = a.n(Re);
-            const Be = Le().stylesheet().selector("node").css({
+            var Ye = a(2393),
+                Xe = a.n(Ye);
+            const Ge = Xe().stylesheet().selector("node").css({
                     content: "data(id)",
                     "background-color": "#4286f4",
                     "font-size": "14px"
                 }).selector(".selected").css({
                     "background-color": "#ff5555",
                     "border-color": "#ff5555",
                     "font-size": "14px"
@@ -1379,50 +1392,50 @@
                     label: "data(label)",
                     "text-rotation": "autorotate",
                     "text-margin-x": "-8px",
                     "text-margin-y": "-8px",
                     color: "gray",
                     "font-size": "12px"
                 }),
-                Ye = {
+                Je = {
                     animate: !0,
                     randomize: !0
                 };
 
-            function Xe(e, t) {
+            function et(e, t) {
                 if (e.length != t.length) return !0;
                 for (let a = 0; a < e.length; a++)
                     if (e[a].id != t[a].id || e[a].label != t[a].label) return !0;
                 return !1
             }
-            const Ge = (0, l.aZ)({
+            const tt = (0, l.aZ)({
                     name: "cgraph",
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
                         return {
                             cy: null,
-                            style: Be,
-                            layoutOptions: Ye,
+                            style: Ge,
+                            layoutOptions: Je,
                             selectedNodes: [],
                             selectedEdges: [],
                             oldNodes: [],
                             oldEdges: [],
                             shiftKey: !1
                         }
                     },
                     beforeUnmount() {
                         window.removeEventListener("keydown", this.handleKeyDown), window.removeEventListener("keyup", this.handleKeyUp)
                     },
                     mounted() {
                         window.addEventListener("keydown", this.handleKeyDown), window.addEventListener("keyup", this.handleKeyUp);
-                        let e = Le()({
+                        let e = Xe()({
                                 container: this.$refs.cy,
                                 elements: {
                                     nodes: this.nodes,
                                     edges: this.edges
                                 },
                                 style: this.style
                             }),
@@ -1472,15 +1485,15 @@
                         },
                         value() {
                             return this.data.value
                         }
                     },
                     methods: {
                         sendMessage(e, t) {
-                            j([this.pdata["name"], this.data["name"], e, t])
+                            S([this.pdata["name"], this.data["name"], e, t])
                         },
                         handleKeyDown(e) {
                             "Shift" == e.key && (this.shiftKey = !0)
                         },
                         handleKeyUp(e) {
                             "Shift" == e.key && (this.shiftKey = !1)
                         },
@@ -1544,15 +1557,15 @@
                                 for (let t of e) a.edges("[id='" + t + "']").addClass("highlighted")
                             }
                         },
                         data: {
                             handler(e, t) {
                                 let a = e.value,
                                     l = !1;
-                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Xe(e.nodes, this.oldNodes) && (l = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Xe(e.edges, this.oldEdges) && (l = !0, this.oldEdges = e.edges), l && null != this.cy) {
+                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), et(e.nodes, this.oldNodes) && (l = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), et(e.edges, this.oldEdges) && (l = !0, this.oldEdges = e.edges), l && null != this.cy) {
                                     this.cy.json({
                                         elements: {
                                             nodes: this.nodes,
                                             edges: this.edges
                                         }
                                     });
                                     let e = this.data.method;
@@ -1569,53 +1582,53 @@
                             this.cy.style(e)
                         },
                         layoutOptions(e) {
                             this.cy.layout(e).run()
                         }
                     }
                 }),
-                Je = (0, N.Z)(Ge, [
-                    ["render", Ie]
+                at = (0, P.Z)(tt, [
+                    ["render", Be]
                 ]),
-                et = Je;
+                lt = at;
 
-            function tt(e, t, a, i, n, o) {
+            function st(e, t, a, i, n, o) {
                 const d = (0, l.up)("v-chart");
                 return (0, l.wg)(), (0, l.j4)(d, {
                     ref: "chart",
                     option: n.options,
                     style: (0, s.j5)(a.styleSize),
                     autoresize: !0
                 }, null, 8, ["option", "style"])
             }
-            var at = a(7559),
-                lt = a(4447),
-                st = a(1006),
-                it = a(3526),
-                nt = a(763),
-                ot = a(546),
-                dt = a(6902),
-                rt = a(2826),
-                ct = a(5256),
-                ht = a(3825),
-                ut = a(8825);
-            (0, nt.D)([lt.N, st.N, it.N]), (0, nt.D)([ot.N, dt.N, rt.N, ct.N, ht.N]);
-            let pt = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"];
-            const gt = {
+            var it = a(7559),
+                nt = a(4447),
+                ot = a(1006),
+                dt = a(3526),
+                rt = a(763),
+                ct = a(546),
+                ht = a(6902),
+                ut = a(2826),
+                pt = a(5256),
+                gt = a(3825),
+                mt = a(8825);
+            (0, rt.D)([nt.N, ot.N, dt.N]), (0, rt.D)([ct.N, ht.N, ut.N, pt.N, gt.N]);
+            let ft = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"];
+            const yt = {
                     name: "linechart",
                     components: {
-                        VChart: at.ZP
+                        VChart: it.ZP
                     },
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
-                        const e = (0, ut.Z)();
+                        const e = (0, mt.Z)();
                         return {
                             $q: e,
                             model: !1,
                             options: {
                                 responsive: !0,
                                 maintainAspectRatio: !1,
                                 legend: {
@@ -1687,58 +1700,58 @@
                             let s = [];
                             for (let n = 0; n < l.length; n++) l[n] = "i" == l[n] ? -1 : parseInt(l[n]), s.push([]), n && (this.options.series.push({
                                 name: t[l[n]],
                                 type: "line",
                                 symbol: "none",
                                 sampling: "lttb",
                                 itemStyle: {
-                                    color: pt[n]
+                                    color: ft[n]
                                 },
                                 data: s[n]
                             }), this.options.legend.data.push(t[l[n]]));
                             this.options.xAxis.data = s[0];
                             let i = this.data.rows;
                             for (let n = 0; n < i.length; n++)
                                 for (let e = 0; e < l.length; e++) s[e].push(-1 == l[e] ? n : i[n][l[e]]);
                             this.$refs.chart.setOption(this.options), this.$refs.chart.chart.on("click", (e => alert("!")))
                         }
                     },
                     mounted() {
                         this.calcSeries()
                     }
                 },
-                mt = (0, N.Z)(gt, [
-                    ["render", tt]
+                wt = (0, P.Z)(yt, [
+                    ["render", st]
                 ]),
-                ft = mt;
+                bt = wt;
 
-            function yt(e) {
+            function kt(e) {
                 let t = new FormData;
                 t.append("image", e);
                 let a = new XMLHttpRequest;
                 a.open("POST", k, !0), a.onload = function() {
                     200 === this.status ? console.log(this.response) : console.error(a)
                 }, a.send(t)
             }
-            const wt = (0, l.aZ)({
+            const vt = (0, l.aZ)({
                 name: "element",
                 components: {
-                    utable: Te,
-                    cgraph: et,
-                    linechart: ft
+                    utable: Ie,
+                    cgraph: lt,
+                    linechart: bt
                 },
                 methods: {
                     log(e) {
                         console.log(e)
                     },
                     onAdded(e) {
                         0 !== e.length && (0 !== this.fileArr.length ? (this.$refs.uploaderRef.removeFile(this.fileArr[0]), this.fileArr.splice(0, 1, e[0])) : this.fileArr.push(e[0]))
                     },
                     sendMessage(e, t) {
-                        j([this.pdata["name"], this.data["name"], e, t])
+                        S([this.pdata["name"], this.data["name"], e, t])
                     },
                     pressedEnter() {
                         "update" in this.data && this.sendMessage("update", this.value)
                     },
                     updateDom(e) {
                         let t = e.files.length;
                         t && this.sendMessage("changed", e.xhr.responseText)
@@ -1749,15 +1762,15 @@
                     switchValue() {
                         this.value = !this.value
                     },
                     setValue(e) {
                         this.value = e
                     },
                     complete(e, t, a) {
-                        "" != e && Z(this, e, (e => t((() => {
+                        "" != e && M(this, e, (e => t((() => {
                             this.options = e
                         }))))
                     },
                     lens() {
                         h.lens(this.data)
                     },
                     toggleCamera() {
@@ -1790,15 +1803,15 @@
                             }), e)
                         }
                         this.isPhotoTaken = !this.isPhotoTaken;
                         const e = this.$refs.canvas.getContext("2d");
                         e.drawImage(this.$refs.camera, 0, 0, 450, 337.5)
                     },
                     downloadImage() {
-                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(yt, "image/jpeg")
+                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(kt, "image/jpeg")
                     },
                     rect() {
                         let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
                         return e.getBoundingClientRect()
                     },
                     geom() {
                         let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
@@ -1813,21 +1826,24 @@
                             right: l.right,
                             top: l.top,
                             scrollHeight: a.scrollHeight,
                             scrollWidth: a.scrollWidth
                         }
                     }
                 },
-                mounted() {
+                updated() {
                     q[this.fullname] = this
                 },
+                mounted() {
+                    q[this.fullname] = this, this.data.focus && this.$refs.inputRef.$el.focus()
+                },
                 data() {
                     return {
                         value: this.data.value,
-                        styleSize: w(this.data),
+                        styleSize: D(`${this.data.name}@${this.pdata.name}`, this.data),
                         host_path: k,
                         options: [],
                         expandedKeys: [],
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
                             backgroundColor: "#027be3",
@@ -1937,53 +1953,53 @@
                         Array.isArray(e) || (e = [0, 0]);
                         let t = this.$refs.inputRef.$el;
                         t.focus();
                         let a = t.getElementsByTagName("textarea");
                         0 == a.length && (a = t.getElementsByTagName("input")), a[0].setSelectionRange(e[0], e[1])
                     },
                     data(e, t) {
-                        this.styleSize || (this.styleSize = w(this.data)), this.value = this.data.value, this.updated = this.value, q[this.fullname] = this
+                        this.styleSize || (this.styleSize = finitStyle(this.data)), this.value = this.data.value, this.updated = this.value, q[this.fullname] = this
                     }
                 }
             });
-            var bt = a(4027),
-                kt = a(9721),
-                vt = a(8886),
-                xt = a(8761),
-                Ct = a(1232),
-                qt = a(5551),
-                _t = a(5869),
-                jt = a(1745),
-                St = a(8430);
-            const zt = (0, N.Z)(wt, [
-                    ["render", je],
-                    ["__scopeId", "data-v-7eaff898"]
+            var xt = a(4027),
+                Ct = a(9721),
+                qt = a(8886),
+                _t = a(8761),
+                jt = a(1232),
+                St = a(5551),
+                zt = a(5869),
+                At = a(1745),
+                Zt = a(8430);
+            const $t = (0, P.Z)(vt, [
+                    ["render", Ae],
+                    ["__scopeId", "data-v-9259610c"]
                 ]),
-                At = zt;
-            L()(wt, "components", {
-                QImg: bt.Z,
-                QIcon: P.Z,
-                QSelect: Ne.Z,
-                QBadge: kt.Z,
-                QCheckbox: Ue.Z,
-                QToggle: vt.Z,
-                QBtn: We.Z,
-                QBtnToggle: xt.Z,
-                QInput: Ee.Z,
-                QScrollArea: Ct.Z,
-                QTree: qt.Z,
-                QSeparator: _t.Z,
-                QUploader: jt.Z,
-                QTooltip: Ke.Z,
-                QSpinnerPuff: St.Z
+                Dt = $t;
+            X()(vt, "components", {
+                QImg: xt.Z,
+                QIcon: L.Z,
+                QSelect: Pe.Z,
+                QBadge: Ct.Z,
+                QCheckbox: Te.Z,
+                QToggle: qt.Z,
+                QBtn: He.Z,
+                QBtnToggle: _t.Z,
+                QInput: Oe.Z,
+                QScrollArea: jt.Z,
+                QTree: St.Z,
+                QSeparator: zt.Z,
+                QUploader: At.Z,
+                QTooltip: Qe.Z,
+                QSpinnerPuff: Zt.Z
             });
-            const Zt = (0, l.aZ)({
+            const Mt = (0, l.aZ)({
                 name: "block",
                 components: {
-                    element: At
+                    element: Dt
                 },
                 data() {
                     return {
                         styleSize: y,
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
@@ -2050,134 +2066,152 @@
                     data: {
                         type: Object,
                         required: !0
                     }
                 },
                 watch: {
                     data(e) {
-                        g && console.log("data update", this.name), this.styleSize = y, C[this.name] = this, this.expanding && (q[this.fullname] = this)
+                        g && console.log("data update", this.name), C[this.name] = this, this.expanding && (this.styleSize = D(this.fullname, this.data), q[this.fullname] = this)
                     }
                 }
             });
-            var Dt = a(151);
-            const Mt = (0, N.Z)(Zt, [
-                    ["render", oe]
+            var Vt = a(151);
+            const Et = (0, P.Z)(Mt, [
+                    ["render", ce]
                 ]),
-                $t = Mt;
-            L()(Zt, "components", {
-                QCard: Dt.Z,
-                QIcon: P.Z,
-                QScrollArea: Ct.Z
+                Kt = Et;
+
+            function Wt() {
+                let e = Z && q.size == _.size;
+                if (e)
+                    for (let [t, a] of Object.entries(q))
+                        if (!_[t]) {
+                            e = !1;
+                            break
+                        } e || (U(), (0, l.Y3)((() => {
+                    requestAnimationFrame((() => {
+                        requestAnimationFrame((() => {
+                            h.visible(!0)
+                        }))
+                    }))
+                })))
+            }
+            X()(Mt, "components", {
+                QCard: Vt.Z,
+                QIcon: L.Z,
+                QScrollArea: jt.Z
             });
-            const Vt = (0, l.aZ)({
+            const Ot = (0, l.aZ)({
                     name: "zone",
                     components: {
-                        block: $t
+                        block: Kt
                     },
                     props: {
                         data: Object
                     },
                     updated(e) {
                         (0, l.Y3)((() => {
                             requestAnimationFrame((() => {
-                                requestAnimationFrame((() => {
-                                    O()
-                                }))
+                                requestAnimationFrame(Wt)
                             }))
                         }))
                     }
                 }),
-                Et = (0, N.Z)(Vt, [
-                    ["render", ee]
+                Qt = (0, P.Z)(Ot, [
+                    ["render", le]
                 ]),
-                Kt = Et,
-                Wt = {
+                Ht = Qt,
+                Ut = {
                     class: "row q-gutter-sm row-md"
                 };
 
-            function Ot(e, t, a, i, n, o) {
+            function Nt(e, t, a, i, n, o) {
                 const d = (0, l.up)("block"),
                     r = (0, l.up)("q-item-label"),
                     c = (0, l.up)("q-space"),
                     h = (0, l.up)("q-btn"),
                     u = (0, l.up)("q-card"),
                     p = (0, l.up)("q-dialog");
                 return (0, l.wg)(), (0, l.j4)(p, {
                     ref: "dialog",
-                    onHide: o.onDialogHide
+                    onHide: o.onDialogHide,
+                    onKeyup: (0, he.D2)(o.pressedEnter, ["enter"])
                 }, {
                     default: (0, l.w5)((() => [(0, l.Wm)(u, {
                         class: "q-dialog-plugin q-pa-md items-start q-gutter-md",
                         bordered: "",
                         style: (0, s.j5)(a.data.internal ? "width: 800px; max-width: 80vw;" : "")
                     }, {
                         default: (0, l.w5)((() => [a.data ? ((0, l.wg)(), (0, l.j4)(d, {
                             key: 0,
                             data: a.data
                         }, null, 8, ["data"])) : (0, l.kq)("", !0), (0, l.Wm)(r, {
                             class: "text-h6"
                         }, {
                             default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(a.data.text ? a.data.text : ""), 1)])),
                             _: 1
-                        }), (0, l._)("div", Wt, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
+                        }), (0, l._)("div", Ut, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
                             class: "col-md-3",
                             label: e,
                             color: a.buttons[0] == e ? "primary" : "secondary",
                             onClick: t => o.sendMessage(e)
                         }, null, 8, ["label", "color", "onClick"])))), 256))])])),
                         _: 1
                     }, 8, ["style"])])),
                     _: 1
-                }, 8, ["onHide"])
+                }, 8, ["onHide", "onKeyup"])
             }
-            const Qt = {
+            const Ft = {
                 props: {
                     data: Object,
                     buttons: Array
                 },
                 components: {
-                    block: $t
+                    block: Kt
                 },
                 emits: ["ok", "hide"],
                 methods: {
                     show() {
                         this.$refs.dialog.show()
                     },
                     sendMessage(e) {
-                        this.data.internal || j([this.data["name"], e]), this.hide()
+                        this.data.internal || S([this.data["name"], e]), this.hide()
                     },
                     hide() {
                         this.$refs.dialog.hide()
                     },
                     onDialogHide() {
                         this.$emit("hide")
                     },
+                    pressedEnter() {
+                        this.sendMessage(this.buttons[0])
+                    },
                     onOKClick() {
                         this.$emit("ok"), this.hide()
                     },
                     onCancelClick() {
                         this.hide()
                     }
                 }
             };
-            var Ht = a(5926),
-                Ut = a(2025);
-            const Nt = (0, N.Z)(Qt, [
-                    ["render", Ot]
+            var Tt = a(5926),
+                Pt = a(2025);
+            const Rt = (0, P.Z)(Ft, [
+                    ["render", Nt]
                 ]),
-                Ft = Nt;
-            L()(Qt, "components", {
-                QDialog: Ht.Z,
-                QCard: Dt.Z,
-                QItemLabel: I.Z,
-                QSpace: Ut.Z,
-                QBtn: We.Z
+                It = Rt;
+            X()(Ft, "components", {
+                QDialog: Tt.Z,
+                QCard: Vt.Z,
+                QItemLabel: B.Z,
+                QSpace: Pt.Z,
+                QBtn: He.Z
             });
-            let Tt = null;
-            const Pt = (0, l.aZ)({
+            let Lt = null;
+            const Bt = (0, l.aZ)({
                 name: "MainLayout",
                 data() {
                     return {
                         leftDrawerOpen: !1,
                         menu: [],
                         tab: "",
                         tooldata: {
@@ -2187,41 +2221,44 @@
                         statusConnect: !1,
                         screen: {
                             blocks: []
                         }
                     }
                 },
                 components: {
-                    menubar: Y,
-                    zone: Kt,
-                    element: At
+                    menubar: J,
+                    zone: Ht,
+                    element: Dt
                 },
                 created() {
-                    _(this)
+                    j(this)
                 },
                 unmounted() {
                     window.removeEventListener("resize", this.onResize)
                 },
                 methods: {
                     toggleLeftDrawer() {
                         this.leftDrawerOpen = !this.leftDrawerOpen
                     },
                     tabclick(e) {
-                        j(["root", e])
+                        S(["root", e])
+                    },
+                    visible(e) {
+                        this.$refs.page.$el.style.visibility = e ? "" : "hidden"
                     },
                     onResize(e) {
-                        g && console.log("window has been resized", window.innerHeight, window.innerWidth), W()
+                        g && console.log("window has been resized", window.innerHeight, window.innerWidth), H()
                     },
                     lens(e) {
                         let t = {
                                 title: "Photo lens",
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0,
-                                component: Ft
+                                component: It
                             },
                             {
                                 height: a,
                                 ...l
                             } = e;
                         l.width = 750;
                         let s = {
@@ -2240,80 +2277,80 @@
                         let a = t,
                             l = {
                                 message: e,
                                 type: t,
                                 position: "top",
                                 icon: a
                             };
-                        "progress" == t ? null == Tt ? (l = {
+                        "progress" == t ? null == Lt ? (l = {
                             group: !1,
                             timeout: 0,
                             spinner: !0,
                             type: "info",
                             message: e || "Progress..",
                             position: "top",
                             color: "secondary"
-                        }, Tt = this.$q.notify(l)) : null == e ? (Tt(), Tt = null) : (l = {
+                        }, Lt = this.$q.notify(l)) : null == e ? (Lt(), Lt = null) : (l = {
                             caption: e
-                        }, Tt(l)) : ("error" == t && l.type, this.$q.notify(l))
+                        }, Lt(l)) : ("error" == t && l.type, this.$q.notify(l))
                     },
                     error(e) {
                         this.notify(e, "error")
                     },
                     info(e) {
                         this.notify(e, "info")
                     },
                     processMessage(e) {
-                        if ("screen" == e.type) this.screen.name != e.name && A(), D(), this.screen = e, this.menu = e.menu.map((e => ({
+                        if ("screen" == e.type) V(), this.screen.name != e.name && ($(!1), this.visible(!1)), this.screen = e, this.menu = e.menu.map((e => ({
                             name: e[0],
                             icon: e[1],
                             order: e[2]
                         }))), this.tab = this.screen.name;
                         else if ("dialog" == e.type) {
                             let t = {
                                 title: e.name,
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0
                             };
-                            t.component = Ft, t.componentProps = {
+                            t.component = It, t.componentProps = {
                                 data: e.content ? e.content : e,
                                 buttons: e.buttons
                             }, this.$q.dialog(t)
-                        } else if ("answer" == e.type) V(e);
+                        } else if ("answer" == e.type) W(e);
                         else {
-                            e.updates && $(e.updates);
+                            e.updates && K(e.updates);
                             let t = !1;
                             ["error", "progress", "warning", "info"].includes(e.type) && (this.notify(e.value, e.type), t = !0), t || e.updates || (this.error("Invalid data came from the server! Look the console."), console.log(`Invalid data came from the server! ${e}`))
                         }
-                        Tt && "progress" != e.type && this.notify(null, "progress")
+                        Lt && "progress" != e.type && this.notify(null, "progress")
                     }
                 },
                 mounted() {
                     window.addEventListener("resize", this.onResize)
                 }
             });
-            var It = a(9214),
-                Rt = a(3812),
-                Lt = a(9570),
-                Bt = a(7547),
-                Yt = a(3269),
-                Xt = a(2652),
-                Gt = a(4379);
-            const Jt = (0, N.Z)(Pt, [
+            var Yt = a(9214),
+                Xt = a(3812),
+                Gt = a(9570),
+                Jt = a(7547),
+                ea = a(3269),
+                ta = a(2652),
+                aa = a(4379);
+            const la = (0, P.Z)(Bt, [
                     ["render", o]
                 ]),
-                ea = Jt;
-            L()(Pt, "components", {
-                QLayout: It.Z,
-                QHeader: Rt.Z,
-                QToolbar: Lt.Z,
-                QBtn: We.Z,
-                QItemLabel: I.Z,
-                QTabs: Bt.Z,
-                QTab: Yt.Z,
-                QPageContainer: Xt.Z,
-                QPage: Gt.Z
+                sa = la;
+            X()(Bt, "components", {
+                QLayout: Yt.Z,
+                QHeader: Xt.Z,
+                QToolbar: Gt.Z,
+                QBtn: He.Z,
+                QItemLabel: B.Z,
+                QTabs: Jt.Z,
+                QTab: ea.Z,
+                QPageContainer: ta.Z,
+                QPage: aa.Z
             })
         }
     }
 ]);
```

### Comparing `unigui-1.8.5/unigui/web/js/430.591e9a73.js` & `unigui-1.9.0/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.8.5/unigui/web/js/vendor.3076c5e7.js` & `unigui-1.9.0/unigui/web/js/vendor.3076c5e7.js`

 * *Files identical despite different names*

### Comparing `unigui-1.8.5/unigui/web/js/app.e17901f8.js` & `unigui-1.9.0/unigui/web/js/app.fb1ab18a.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(164)]).then(r.bind(r, 4164)),
+                        component: () => Promise.all([r.e(736), r.e(615)]).then(r.bind(r, 9615)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -158,25 +158,25 @@
                 get: t[n]
             })
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, n) => (r.f[n](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
-            164: "2b869daf",
             193: "283445be",
-            430: "591e9a73"
+            430: "591e9a73",
+            615: "04cc6ad4"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
-            164: "06cedad1",
+            615: "3024385a",
             736: "191faa77"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
@@ -260,15 +260,15 @@
                 e(n, l, o, a)
             })),
             o = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                164: 1
+                615: 1
             };
             o[e] ? t.push(o[e]) : 0 !== o[e] && r[e] && t.push(o[e] = n(e).then((() => {
                 o[e] = 0
             }), (t => {
                 throw delete o[e], t
             })))
         }
```

### Comparing `unigui-1.8.5/unigui/web/js/193.283445be.js` & `unigui-1.9.0/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.8.5/unigui/web/index.html` & `unigui-1.9.0/unigui/web/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.3076c5e7.js></script><script defer src=js/app.e17901f8.js></script><link href=css/vendor.191faa77.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.3076c5e7.js></script><script defer src=js/app.fb1ab18a.js></script><link href=css/vendor.191faa77.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.8.5/LICENSE` & `unigui-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.8.5/PKG-INFO` & `unigui-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.8.5
+Version: 1.9.0
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.8.5/README.md` & `unigui-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `unigui-1.8.5/unigui.egg-info/PKG-INFO` & `unigui-1.9.0/unigui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.8.5
+Version: 1.9.0
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.8.5/unigui.egg-info/SOURCES.txt` & `unigui-1.9.0/unigui.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,27 +13,30 @@
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/164.06cedad1.css
+unigui/web/css/615.3024385a.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.191faa77.css
+unigui/web/css/vendor.191faa77.css.gz
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
 unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
-unigui/web/js/164.2b869daf.js
 unigui/web/js/193.283445be.js
 unigui/web/js/430.591e9a73.js
-unigui/web/js/app.e17901f8.js
-unigui/web/js/vendor.3076c5e7.js
+unigui/web/js/615.04cc6ad4.js
+unigui/web/js/615.04cc6ad4.js.gz
+unigui/web/js/app.fb1ab18a.js
+unigui/web/js/vendor.3076c5e7.js
+unigui/web/js/vendor.3076c5e7.js.gz
```

