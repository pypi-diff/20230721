# Comparing `tmp/discohooker-1.0.3.tar.gz` & `tmp/discohooker-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discohooker-1.0.3.tar", last modified: Fri Jul 21 07:49:23 2023, max compression
+gzip compressed data, was "discohooker-1.0.4.tar", last modified: Fri Jul 21 07:56:08 2023, max compression
```

## Comparing `discohooker-1.0.3.tar` & `discohooker-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-21 07:49:23.977807 discohooker-1.0.3/
--rw-r--r--   0 runner    (1000) runner    (1000)     1066 2023-07-17 08:42:29.000000 discohooker-1.0.3/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1472 2023-07-21 07:49:23.977807 discohooker-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1008 2023-07-21 04:47:01.000000 discohooker-1.0.3/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-21 07:49:23.973807 discohooker-1.0.3/discohooker/
--rw-r--r--   0 runner    (1000) runner    (1000)      109 2023-07-20 07:47:04.000000 discohooker-1.0.3/discohooker/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3723 2023-07-20 07:40:11.000000 discohooker-1.0.3/discohooker/embed.py
--rw-r--r--   0 runner    (1000) runner    (1000)      474 2023-07-21 04:07:46.000000 discohooker-1.0.3/discohooker/errors.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3176 2023-07-21 07:49:02.000000 discohooker-1.0.3/discohooker/message.py
--rw-r--r--   0 runner    (1000) runner    (1000)      474 2023-07-21 04:24:20.000000 discohooker-1.0.3/discohooker/tasks.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3387 2023-07-21 07:48:33.000000 discohooker-1.0.3/discohooker/webhook.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-21 07:49:23.973807 discohooker-1.0.3/discohooker.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1472 2023-07-21 07:49:23.000000 discohooker-1.0.3/discohooker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2023-07-21 07:49:23.000000 discohooker-1.0.3/discohooker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-21 07:49:23.000000 discohooker-1.0.3/discohooker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-07-21 07:49:23.000000 discohooker-1.0.3/discohooker.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-21 07:49:23.000000 discohooker-1.0.3/discohooker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      489 2023-07-20 07:25:45.000000 discohooker-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-21 07:49:23.977807 discohooker-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      712 2023-07-21 07:49:13.000000 discohooker-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-21 07:56:08.489689 discohooker-1.0.4/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1066 2023-07-17 08:42:29.000000 discohooker-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1472 2023-07-21 07:56:08.489689 discohooker-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1008 2023-07-21 04:47:01.000000 discohooker-1.0.4/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-21 07:56:08.489689 discohooker-1.0.4/discohooker/
+-rw-r--r--   0 runner    (1000) runner    (1000)      109 2023-07-20 07:47:04.000000 discohooker-1.0.4/discohooker/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3723 2023-07-20 07:40:11.000000 discohooker-1.0.4/discohooker/embed.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      474 2023-07-21 04:07:46.000000 discohooker-1.0.4/discohooker/errors.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3184 2023-07-21 07:55:36.000000 discohooker-1.0.4/discohooker/message.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      474 2023-07-21 04:24:20.000000 discohooker-1.0.4/discohooker/tasks.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3387 2023-07-21 07:48:33.000000 discohooker-1.0.4/discohooker/webhook.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-21 07:56:08.489689 discohooker-1.0.4/discohooker.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1472 2023-07-21 07:56:08.000000 discohooker-1.0.4/discohooker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2023-07-21 07:56:08.000000 discohooker-1.0.4/discohooker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-21 07:56:08.000000 discohooker-1.0.4/discohooker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-07-21 07:56:08.000000 discohooker-1.0.4/discohooker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-21 07:56:08.000000 discohooker-1.0.4/discohooker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      489 2023-07-20 07:25:45.000000 discohooker-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-21 07:56:08.489689 discohooker-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      712 2023-07-21 07:55:56.000000 discohooker-1.0.4/setup.py
```

### Comparing `discohooker-1.0.3/LICENSE` & `discohooker-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `discohooker-1.0.3/PKG-INFO` & `discohooker-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discohooker
-Version: 1.0.3
+Version: 1.0.4
 Summary: A easy PyPI to send Discord Webhook!
 Home-page: https://replit.com/@MAX110331/discohooker
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `discohooker-1.0.3/README.md` & `discohooker-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `discohooker-1.0.3/discohooker/embed.py` & `discohooker-1.0.4/discohooker/embed.py`

 * *Files identical despite different names*

### Comparing `discohooker-1.0.3/discohooker/message.py` & `discohooker-1.0.4/discohooker/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         for embed in embeds:
             _embeds.append(embed._to_dict)
         if content == None:
             _content=""
         else:
             _content=content
         _jdata={"content": _content, "embeds": _embeds}
-        response=requests.patch(f"{self.weburl}/messages/{message_id}", data=_jdata)
+        response=requests.patch(f"{self.webhook.weburl}/messages/{message_id}", data=_jdata)
         if response.status_code == 304:
             raise Errors.APIError("The entity was not modified (no action was taken).")
         elif response.status_code == 429:
             raise Errors.APIError("You are being rate limited, see https://discord.com/developers/docs/topics/rate-limits.")
         elif response.status_code == 400:
             raise Errors.APIError("The request was improperly formatted, or the server couldn't understand it.(Bad Request)")
         elif response.status_code == 401:
```

### Comparing `discohooker-1.0.3/discohooker/webhook.py` & `discohooker-1.0.4/discohooker/webhook.py`

 * *Files identical despite different names*

### Comparing `discohooker-1.0.3/discohooker.egg-info/PKG-INFO` & `discohooker-1.0.4/discohooker.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discohooker
-Version: 1.0.3
+Version: 1.0.4
 Summary: A easy PyPI to send Discord Webhook!
 Home-page: https://replit.com/@MAX110331/discohooker
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `discohooker-1.0.3/setup.py` & `discohooker-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="discohooker",
-    version="1.0.3",
+    version="1.0.4",
     author="MaxPython110331",
     author_email="max.gamil110331@gmail.com",
     description="A easy PyPI to send Discord Webhook!",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://replit.com/@MAX110331/discohooker",
```

